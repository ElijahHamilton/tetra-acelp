# tetra-acelp
Basic encoder/decoder programs for the full-rate Tetra codec.
These example programs are written by myself. However, the actual codec code is from [outerplane.](https://github.com/outerplane/tetra-codec)

# Building
You can build the programs using `./build.sh`.

Or for speed:

`gcc -Icodec/ -Ofast encoder.c codec/*.c -o encoder`

`gcc -Icodec/ -Ofast decoder.c codec/*.c -o decoder`

No significant codec changes occur when compiling with `-Ofast`.

# Info
The codec itself opperates at 4566.66666... bit/s second. Although, my example programs pad the bitrate to 4800 bit/s.
