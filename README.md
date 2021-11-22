# Data-File-Handling-Notes
In This we will get the notes of DATA FILE HANDLING

Transient :- These are the programs which runs for a short time and produce some output , but when they end their data disappears .
Persistent :- These are the programs which runs for a long time , They keep atleast some part of the data in permanent storage ( example :- Hardware ).

Data is packaged up on the storage devices as data structure called :- Files .

RAM :- Random Access Memory
ROM :- Read Only Memory .

Each line is terminated by the special character called :- EOL ( End of Line ) .
ASCII :- American Standard Code for Information Interchange .

Binary Files :- are also used to store the binary data such as ( Images , Audio Files , Video Files etc. .) .

open() :- For opening a files .
 > MODES FOR OPENING A FILE :-
 1 )- read (r) :- to read a file.
 2 )- write (w) :- to write to the file .
 3 )- append (a) :- to read at the end of the file .
 
flush() :- function of the file object is use to force transfer of data from buffer to file .

NOTE :- >>> When you open a file in the readmode the file must exists in the folder , otherwise the program will show   FileNotFoundError .

  SOME FILE MODES :- 
1 )- r :- opens a file for reading only ..
2 )- rb :- opens a file for reading only in the binary file .
3 )- r+ :- opens the file for both reading and writing .
4 )- rb+ :- Opens the binary file for both reading and writting purposes .
5 )- wb :- Opens a file for writing only in the Binary File .
6 )- w :- opens a file for writing only in the text file .
7 )- a :- opens a file for appending .
8 )- ab :- opens a file for appending in the binary format .
9 )- a+ :- opens a file for both appending and reading in the text format .
10 )- ab+ :- opens a file for both appending and reading in the binary format .



close () :- This method is used to close the file object , after which no more writting can be done .


READING FROM THE FILE :- 
There are the various types of the reading methods some are as follows :-
 1 )- read () :- To read tye entire data from the file.
 2 )- read (n) :- To read "n" characters from the file.
 3 )- readline () :- To read only one line from the file .
 4 )- readlines () :- To read all lines from the data  _ This will store in the form of the list .
 5 )- readable () :- This will returns True if the file is readable else it will returns False .
 
 
Syntax of the read function :-
fileObject.read ()




WRITING IN THE FILE :-
They are also of the two types :-
 1)- write () :- This method takes a string ( as parameter ) and writes it in the text file in a single line .
     Syntax :- fileObject.write (string)
 For storing the numeric data into the file the string conversion is required .
 This can be used for writing a string at a time .
 This can't be used for writing a list, tuple , etc.. into a file .
 
 2 )- writelines()
 
 
 
 APPENDING A FILE :- 
 This is used for opening a file for writing , if exists , This append the data at the end of the file .
        SYNTAX :-
  <file_object> = open(<filename> , "a" )
 
 
 Serilisation :- This is the Process of transforming data or object in RAM to a stram of bytes called _ Bytestreams .
   Serilisation process is also called Pickling.
 
 Pickling :- refers to the process of converting the structure to a bytestream before writing to the file .
