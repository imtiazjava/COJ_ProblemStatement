# COJ_ProblemStatement <br/>

# WOrking With Objects<br/>

<hr>

<b>Batsman_01.java</b>
<p>
<h3>SPECIFICATIONS</h3>

1) Add the following attributes to the class "Batsman".

"name" of type String
"runScored" of type int
"centuries" of type int
"halfCenturies" of type int
"ballsFaced" of type int
"fours" of type int
"sixes" of type int

NOTE: No access modifier should be mentioned against the attributes.

2) Add the following method to class Batsman

Name of the method: setData() with following arguments.

"name" of type String
"runsScored" of type int
"centuries" of type int
"halfCenturies" of type int
"ballsFaced" of type int
"fours" of type int
"sixes" of type int
Return type: void

TO DO: Initialize the respective instance members of the class with the given arguments.   
   
3) Add the below method to class Batsman

Name of the method: getStrikeRate() with no arguments. 

Return type: float

TO DO: Calculate strike rate ( runsScored*100) / ballsFaced  to two decimal values and return it. 

4) Add the below method to class Batsman

Name of the method:  getRunsScoredInBoundaries() with no arguments.

Return type: int

TO DO: Calculate the runs scored in boundaries ( 4 * fours + 6 * sixes ) and return it.
</p>

<hr/>
<b>Batsman_02.java</b>
<p>
   
 <h3>SPECIFICATIONS</h3>

1) Declare the data members as private in class Batsman. 

2) Add default Constructor to class Batsman. 

TO DO: NA

Access modifier: public

3) Add parameterized Constructor to class "Batsman", with following arguments: 
"name" of type String
"runsScored" of type int
"centuries" of type int
"halfCenturies" of type int
"ballsFaced" of type int
"fours" of type int
"sixes" of type int
TO DO: Initialize the instance members of a class with given arguments

Access modifier: public

4) Add getter and setter methods with public access modifier for every attribute in class Batsman 
</p>
<hr/>
<b>Batsman_03.java</b>
<p>
 <h3>SPECIFICATIONS</h3>
1) Add the following variables

"id" of type int
"idGenerator" of type int, specify the modifier 'static' and initialize it to 100000
NOTE: Access modifier should be 'private' for both the above-listed variables 

2) Auto-generate the id, which uniquely identifies Batsman 

TO DO: Pre-increment "idGenerator" and assign it to instance member "id" in both the constructors, default and parameterized 

3) Add getter method to field "id" 
</p>

<hr/>
<b>Batsman_04.java</b>
<p>
 <h3>SPECIFICATIONS</h3>
1) Add the following attributes to class Espncricinfo
"SIZE" which is a constant of type int and initialize it to 50
"batsmans" of type Batsman[]
"noOfBatsmen" of type int
NOTE: private access specifier should be mentioned against the attributes.


2) Add the below method to class Espncricinfo.

Name of the method: getBatsmans() with no arguments. 

Return type: Batsman[]. 

TO DO: Returns an array of type Batsman. 

3) Add the below method to class Espncricinfo.

Name of the method: getNoOfBatsmen() with no arguments. 

Return type: int

TO DO: Return the value of the variable "noOfBatsmen". 

4) Add the below method to class Espncricinfo

Name of the method: addBatsman()

Arguments:
"name" of type String
"runsScored" of type int
"centuries" of type int
"halfCenturies" of type int
"ballsFaced" of type int
"fours" of type int
"sixes" of type int
Return Type: int

TO DO: If the value of variable "noOfBatsman" is less than SIZE-1, add to the array and return an id of  added Batsman, else return zero. 

5) Add the below method to class Espncricinfo

Name of the method: updateBatsmanStats()

Arguments:

"id" of type int
"runsScored" of type int
"fours" of type int
"sixes" of type int
"ballsFaced" of type int
Return type: Batsman

TO DO: If batsmanId found, update stats and return object, else return "null" 

6) Add the below method to class Espncricinfo

Name of the method: getBatsman()

Arguments:
"batsmanId" of type int
Return Type: Batsman

TO DO: If batsmanId found, return object of type Batsman, else return "null"

</p>

<hr/>

# Generalization and Specialization of Objects<br/>

<b>Player_01.java</b>
<p>
 <h3>SPECIFICATIONS</h3>
SPECIFICATIONS
1) Add a parameterized constructor to class "Batsman", which initializes the following attributes
"name" of type String
"runsScored" of type int
"centuries" of type int
"halfCenturies" of type int
"sixes" of type int
"fours" of type int
"ballsFaced" of type int

2) Add a parameterized constructor to class "Bowler", which initializes the following attributes
"name" of type String
"ballsBowled" of type int
"runsLeaked" of type int
"wickets" of type int

</p>

<hr/>
<b>Player_02.java</b>
<p>
 <h3>SPECIFICATIONS</h3>

1) Add the below method to class "Player". 

Name of the method: toString() with no arguments. 

Return type: String

TO DO: Concatenate all the instance members of class Player and return.

2) Add the below method to class Batsman 

Name of the method: toString() with no arguments. 

Return type: String

TO DO: Concatenate all the instance members of class Batsman and Player and return. 

3) Add the below method to class Bowler 

Name of the method: toString() with no arguments. 

Return type: String

TO DO: Concatenate all the instance members of class Bowler and Player and return. 

</p>

<hr/>
<b>Player_03.java</b>
<p>
 <h3>SPECIFICATIONS</h3>

1) Add the below abstract method to class Player 

Name of the method: calcStrikeRate() with no arguments. 

Return type: float

TO DO: NA 

Access modifier: public

2) Add the inherited abstract method to class Batsman 

Name of the method: calcStrikeRate() with no arguments. 

Return type: float

TO DO: Calculate strike rate ( runsScored / ballsFaced ) to two decimal values and return.

3) Add the inherited abstract method to class Bowler 

Name of the method: calcStrikeRate() with no arguments. 

Return type: float

TO DO: Calculate strike rate ( ballsBowled / wickets ) to two decimal values and return. 

</p>

<hr/>
<b>Player_04.java</b>
<p>
 <h3>SPECIFICATIONS</h3>

1) Player class should implement the Comparable interface. 

2) Add the inherited abstract method. 

TO DO: Define the logic to compare the objects of type Player by name.
 
</p>

<hr/>

# Managing Multiple Objects<br/>

<b>SortedOrder_01.java</b>
<p>
 <h3>SPECIFICATIONS</h3>
A) Batsman: 
   1. Defined the constructors and toString methods.
   2. Override the compareTo method.
B) SortedOrder01:
   1. Define the sortByName method.

SPECIFICATIONS:
Name of the method: compareTo(Batsman)// takes Batsman class object as an argument, which compares with the another object of the same class with the name.
Arguments: One Argument of Batsman.
Return type: int 
  

Name of the method: sortByName(List<Batsman>)// return the list which contains batsman object in sorted order by name.
Arguments: One Argument of List<Batsman>
Return Type: A List<Batsman>

</p>
<hr/>
<b>UniqueLetter_02.java</b>
<p>
 <h3>SPECIFICATIONS</h3>

Write the methods with the following specifications:

Name of the method: getUniqueLetters(String)// takes a string value as an argument and returns the Set which contains the unique letters in ascending order.
Arguments: One argument of String type.
Return type: A Set contains all unique letters
SPECIFICATIONS:
If the given String value is null, return the empty Set.
If the String contains leading and trailing white space, remove the spaces.
If the String contains any other letters excluding alphabets or digits, return a Set which contains only alphabets and digits.
In all other cases return the Set which contains all unique letters in ascending order.
Example:

Let String str = "ENGINEERING"

       Output: E, G, I, N, R

        str = "engineering123"

        Output: 1, 2, 3, e, g, i, n, r

         str = ""Aa1Bb2Cc3Dd4"

         Output: 1, 2, 3, 4, A, B, C, D, a, b, c, d

         str = "ABC1@3$5&"

         Output: 1, 3, 5, A, B, C
</p>

<hr/>
<b>CharFrequence_03.java</b>
<p>
 <h3>SPECIFICATIONS</h3>
Write a program to count the frequency of each letter in a given String.

Name of the method: frequencyCount(String)// takes a string value as argument and returns the Map which contains the frequency count of characters.
Arguments: One Argument of String type.
Return Type: A Map<Character, Integer> value
SPECIFICATIONS:
    If the given string value is null, return the empty Map.
    If the string contains leading and trailing white space, remove the spaces.
    If the given string contains lower case letters convert them to upper case.
    If the given string contains any other letter excluding alphabets, return the Map which contains the count of alphabets.
    If the given string don't contains any alphabets, return the empty Map.
    In all other cases return the Map which contains all characters frequency.
Note: 
1. The key value must be in upper case only.
2. The Elements in the map should appear in the same order the letters appear in the string.

Examples:

Let String str = "ELEMENTS" or "elements" or "EleMenTs" or "1EleM2eNTS" or "E#LEMEN$TS1"

Output: A Map which contains the elements (E=3, L=1, M=1, N=1, T=1, S=1)

Let String str = "23#$%#65" or "  "

Output: return an empty Map
</p>

<hr/>
<b>Anagrams_04.java</b>
<p>
 <h3>SPECIFICATIONS</h3>
Write a program to find the set of anagrams from the given String array.

Explanation:
A word or phrase formed by reordering the letters of another word or phrase. 
    Example:
          1. reserved and reversed are anagrams
          2. states and tastes are anagrams
 
Name of the method: findAnagrams(String[])// takes a String array as an argument and returns the list which contains the anagram words separated by COMMA.
Arguments: One Argument of String Array. 
Return Type: A List<String> value 

Note: 
   1. Make sure the input String array is not empty.
   2. The letters in a String must contain only alphabets.

SPECIFICATIONS:
 If two strings contain the same characters with a different case, treat them as anagrams.   Ex: "PART" and "trap" are anagrams.
The anagram words in the list must be in lower case only.
If the String arrays don't contain any anagrams, return an empty list.
In all other cases return the list which contains anagrams separated by COMMA as shown below.
Example: 
  Let String[] words = {"listen", "silent", "elbow", "PART", "panel", "trap", "tensil", "alter", "later", "below"};
  Output:
         listen,silent,tensil
         elbow,below
         part,trap
         alter,later
</p>

<hr/>
# Reading and Writing Data

<hr/>
<b>BatsmanData.java</b>
<p>
 <h3>SPECIFICATIONS</h3>
Write a program which reads batsman data from a file and store in the batsman objects.

Explanation:
Download the file BatsmanData01.java, which contains the Batsman and BatsmanData01 classes:
A) Batsman: 
   1. Defined the constructors and toString methods.
B) BatsmanData01:
   1. Define the readBatsmanData method.

Note:  You must use the sample data file. BatsmanData.txt

SPECIFICATIONS:
Name of the method: readBatsmanData(String)// Read batsman data from a file and add to the batsman object.
Arguments: One Argument of String (File Path)
Return Type: A List<Batsman>
</p>

<hr/>
<b>CopyFile.java</b>
<p>
 <h3>SPECIFICATIONS</h3>
Write a program to copy the content from one file to another file.

Note: Use BufferedReader and BufferedWriter class to copy the content.

Write the methods with the following specifications:

Name of the method: copyFile(String, String)// takes source and dest file path as argument and copy the content, return true if copied else return false.
Arguments: Two Arguments of string.
Return Type: A boolean value  
SPECIFICATIONS:
 If copied the file, return true else return false

</p>

<hr/>
