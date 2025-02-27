# FRPBP

A Lossless Compression Method for VCD Files Based on Signal Function Relationships, Value Prediction, and Bit-Plane Reorganization

## Author:

Zhiqiang He 
Nanjing University of Aeronautics and Astronautics
zhiqiang_he@nuaa.edu.cn


Gang Chen
Nanjing University of Aeronautics and Astronautics
gangchensh@qq.com

## program:

Compress and decompress directly compress VCD files and decompress compressed files.

Compress command
`./compress.exe <vcd file> -comp <compressed file> `

Deompress command
`./compress.exe <compressed file> -decomp <decompressed file> `

Print command
`./compress.exe test.vcd -print `

Verify that the compression is correct:
diff <decompressed file> <`./compress.exe test.vcd -print `>

## Example:

./compress.exe test.vcd -comp comp

./compress.exe comp -decomp decomp

./compress.exe test.vcd -print > print.vcd
diff decomp print.vcd

