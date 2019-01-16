# lz4-68k
Three versions of LZ4 decoders for 68k processors. 
Written by Arnaud Carré
LZ4 technology by Yann Collet ( https://lz4.github.io/lz4/ )

If you're using LZ77 decoder in your demo, you can switch to this for sure. LZ4 has better packing ratio than LZ77 and it depacks faster

The fastest version use 3722 bytes and is suited for CPU without instruction cache ( 68000 )
Prefer lz4_normal.asm for cache instruction CPU ( >= 68020 )

| source code | decoder size | speed factor |
|-|--------------|--------------|
| lz4_smallest.asm | 78 bytes | x 1.0 |
| lz4_normal.asm | 180 bytes | x 1.53 |
| lz4_fastest.asm | 3722 bytes | x 2.36 |

