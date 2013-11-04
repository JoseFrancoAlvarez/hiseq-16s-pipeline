# BIG OTU Pipeline

## Goals

- Streaming: results come out live. Allows you to start doing statistics
  as the analysis progresses.
- Distributed (using TORQUE for now).
- Quality control at each step.
- Capable of analyzing subsets of data.
- 100% Bash + Python 2.7

## Pipeline

1. Split By Barcode.
2. Trim for Quality.
3. Convert to FASTA.
4. Reverse-Complement "right" pair.
5. Split into batches of FASTA files.
6. Submit USEARCH jobs for each FASTA file.

## License

The MIT License (MIT)

Copyright (c) 2013 Austin G. Davis-Richardson

Permission is hereby granted, free of charge, to any person obtaining a
copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be included
in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
