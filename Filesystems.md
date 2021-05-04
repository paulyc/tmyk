# The More You Know About ....
## SD Cards
### Specifically wrt Our Favorite Least Favorite Filesystem (exFAT)
#### c/o exfatutils package
```
 OPTIONS
-b, --boundary-align=alignment
Specifies the alignment for the FAT and the start of the cluster heap.  The alignment argument is spec‐
ified in bytes or may be specified with m/M suffix for mebibytes or k/K suffix for kibibytes and should 
be  a power of two.  Some media like SD cards need this for optimal performance and endurance, in which
case alignment should be set to half of the card's native boundary unit size.   If  the  card's  native 
boundary unit size is not known, refer to the following table of boundary unit sizes recommended by the 
SD Card Association.

Card Capacity Range      Cluster Size   Boundary Unit
──────────────────────────────────────────────────────
            ≤8 MiB           8 KiB          8 KiB
  >8 MiB   ≤64 MiB          16 KiB         16 KiB 
 >64 MiB  ≤256 MiB          16 KiB         32 KiB
>256 MiB    ≤1 GiB          16 KiB         64 KiB  
  >1 GiB    ≤2 GiB          32 KiB         64 KiB  
  >2 GiB   ≤32 GiB          32 KiB          4 MiB 
 >32 GiB  ≤128 GiB         128 KiB         16 MiB
>128 GiB  ≤512 GiB         256 KiB         32 MiB
>512 GiB    ≤2 TiB         512 KiB         64 MiB
```

Or, in a nice Markdown table:

| Card Capacity Range | Cluster Size | Boundary Unit |
| ------------------- |-------------- | ----------------|
|    0     |   ≤8 MiB     |      8 KiB    |      8 KiB|
|  >8 MiB |  ≤64 MiB     |     16 KiB    |     16 KiB |
| >64 MiB | ≤256 MiB     |     16 KiB    |     32 KiB|
|>256 MiB |   ≤1 GiB     |     16 KiB     |    64 KiB | 
|  >1 GiB |   ≤2 GiB     |     32 KiB     |    64 KiB  |
|  >2 GiB |  ≤32 GiB     |     32 KiB     |     4 MiB |
| >32 GiB | ≤128 GiB     |    128 KiB     |    16 MiB|
|>128 GiB | ≤512 GiB     |    256 KiB     |    32 MiB|
|>512 GiB |   ≤2 TiB     |    512 KiB     |    64 MiB|
