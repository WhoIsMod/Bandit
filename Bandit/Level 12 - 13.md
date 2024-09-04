first we have to change the file format to a binary file using the rename command 
`xxd -r data.txt > data`  or any binary tool of your choice

Since the data file is in gzip compression format we use the gunzip tool to uncompress it
`gunzip -c data > data1`
 the next compression format is bzip2 which we use the bunzip2 program to decompress
 `bunzip2 -c data1 > data2`
repeat steps `gunzip -c data2 > data3`
`tar -xf data3`

it gives out a data5.bin file
`tar -xf data5.bin`
`bunzip2 -c data6.bin > data7`
`tar -xf data7`
`gunzip -c data8.bin > data9`
`cat data9`
the key is `FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn`
