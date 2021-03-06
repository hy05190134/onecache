# Changelog

## 2.1.0 (2017-05-05)

- Added Garbage collection (in the background) for the filesystem and memory cache
- Added a new interface `GarbageCollector`. This should be implemented only by cache stores without automatic garbage collection.

## 2.0.1 (2017-05-02)

- Serializer would now refuse to encode/decode values that are already of `[]byte`. For decoding, it must be a pointer to the byte array.
- Fixed wrong usage of protetion with a mutex in the memory store

## 2.0.0 (2017-05-01)

- This was a big update and while it came too soon. It was as a result of some design tradeoff v1.0.0 made.
- The major change was to stop the use of `interface{}` and migrate to `[]byte`. This offers much more type safety.

## 1.0.0 (2017-04-29)

- Initial release
- Stores
 
  - Inmemory
  - Redis
  - Memcached
  - Filesystem

