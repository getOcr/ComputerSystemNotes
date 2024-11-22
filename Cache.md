# Cache

**Block size**: how many bytes there are in each block (a terminology in memory), divide memory address into blocks

**Cache size**: is given in units of bytes or units of blocks, how many bytes or blocks in cache

if block size = K, the **Block number** = A/K, the **Block offset** = A%K

Some matrics: 

average memory access time(AMAT), hit time(HT), miss penalty(MP)

### Direct-Mapped Cache Placement

in order to reduce AMAT

use a hash function

index of cache = block num % cache size

![image-20241122013553519](.\1)