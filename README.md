# NDS-Reference-Values
### Setup
 Download the zip and extract \example, then open \example\data look for tables.csv. If it's missing just add it.
Next go back to \example and run NDS-Reference-Values.exe.

### Registering Tables
 First off we'll get message saying no files are registerd. This is fine just means there are no tables stored in tables.csv. In order to register a file we'll use the command "register" fallowed by the table's name. You're able to seperate the table name's with commas to register multiple. As an example run "register Douglas Fir-Larch.csv". You'll get a message saying the program has registerd douglas fir-larch.csv. In order for the program to read whats in the table we need to run "reload". Finally the program will tell us it has loaded douglas fir-larch.csv. Thats the basics to register and load a table for the program to use. You only need to register a table once. As program saves the registerd tables to tables.csv and loads them when it starts. Try adding a few more but this time all at once. You can find some tables in \data\tables. However DO NOT register Redwood.csv I belive it's incorrectly formated.
The line in question is "Select Structural, open grain","2"" & Wider",1100,625,160,425,1100,1100000,400000. The third value "2"" & Wider" should be an int right? In the next update I will add error handling to the parser. Making errors like this alot easier to find and fix.

### Searching Tables
 Now that we've registered Douglas Fir-Larch.csv we can search through. All we need to do is enter the name it's name "Douglas Fir Larch" without any dashs, caps dont matter. The program will print out a formatted table for us to look through. This is great and all but we can narrow down the search more. Same as last time enter the table but add a dash and a grain "Douglas Fir Larch-Select Structural". The program will narrow down the search to just that line.

### Notes
This is all I have for now but I will be adding more in the future. Please let me know of any bugs you find miss spellings, errors, incorrect formatting, ect.
