# buffer-cache

A simple memory cache using buffers and byte limits

## Usage

```typescript
const cache: BufferCache<number, TestingType> = new BufferCache([[{ id: 1 }]], {
  ttl: 1,
  maxByteSize: 900,
  resizeStrategy: 'LARGEST',
});
```

### Resize strategy

Able to choose between removing largest, first, last of the cache.
