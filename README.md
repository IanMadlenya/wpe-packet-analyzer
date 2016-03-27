# wpe-packet-analyzer (WPA)

![](https://raw.githubusercontent.com/ahvonenj/wpe-packet-analyzer/master/gh-res/wpe-bs.png)

When you have captured network packets with WPE and want to compare similar packets to find deltas and offsets, 
you would often have to fire up Microsoft Excel and get annoyed because:

A) It is hard to paste the packet data into excel (have to save the data into a text file first, to benefit from automatic column separation)  
B) Excel likes to fuck up the column widths and the is not enough space any way  
C) All the comparisons and analyzing must be done manually from scratch every time  
D) Analyzing more than 2 similar packets becomes unintuitive and time consuming

This simple little network packet byte analyzer tries to make analyzing packets captured with WPE a little bit easier and more automatic. 
wpe-packet-analyzer (WPA) automatically finds out packet byte deltas and offsets from given packets and pretty prints them out. 

**Later on, WPA will:**

A) Heuristically find out, if given packets seem to have `common blocks`, such as `time` or `id` bytes at the beginning of the packet  
B) Help to convert hex bytes to decimal and perhaps even back again if needed (ASCII presentation also a possibility, although usually not useful  
C) Assist with marking certain bytes obsolete or socket-breaking  
D) Maybe accept WPE capture files and read input directly from them  
E) Cure cancer and make data mining of software (read: games) not so painful and maybe even fun

**Definition of done:**  
If it takes me no more than 5 minutes to to find the significant bytes,  then this tool has done its job.

![](https://raw.githubusercontent.com/ahvonenj/wpe-packet-analyzer/master/gh-res/wpa-awesome.png)

## Early demo is now available 

http://ahvonenj.github.io/wpe-packet-analyzer/#

Just press the `Analyze packets` button and see the magic happen! You can mouse over the analyzed bytes to highlight them as well as click to copy them straight to your clipboard (if you browser supports it).
