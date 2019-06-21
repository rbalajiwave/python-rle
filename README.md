# python-rle
Convert a PNG file into a human-readable RLE format by using Python 3 and Pillow.

TO RUN:

python png_to_rle.py <inputfilepath> <outputfilepath>


<h3>What is RLE</h3>
According to Wikipedia, RLE stands for "Run-length encoding (RLE)". <br/><br/>
Run-length encoding is a very simple form of lossless data compression in which runs of data (that is, sequences in which the same data value occurs in many consecutive data elements) are stored as a single data value and count, rather than as the original run.
<br/><br/>
<i>For example, this string:</i><br/>
WWWWWWWWWWWWBWWWWWWWWWWWWBBBWWWWWWWWWWWWWWWWWWWWWWWWBWWWWWWWWWWWWWW<br/><br/>
<i>...becomes this after using RLE:</i><br/>
12W1B12W3B24W1B14W<br/><br/>
This script simply converts a binary PNG image into an RLE-type file format.
<h3>Example</h3>
<i>Original image</i><br/>
<img src="https://github.com/anwserman/python-rle/blob/master/input/golfcourse.png">
<i>Sample output</i><br/>
<pre>
#Image Dimensions
Width: 683 
Height: 384 


#Image Palette
255, 0, 128
0, 102, 0
0, 255, 0
66, 255, 66
0, 0, 255
255, 255, 0
128, 128, 128
0, 0, 0

#Pixel Count
0: 42670
1: 48
0: 631
1: 53
0: 627
1: 61
0: 55
2: 55
0: 509
1: 67
0: 48
2: 63


