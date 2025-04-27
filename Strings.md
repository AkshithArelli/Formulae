**Alphanumeric characters include letters and numbers**

function to check whether a character is alpha numeric or not
    public boolean isAlfaNumeric(char ch) {
        return (ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z') 
                || (ch >= '0' && ch <= '9');
    }

**convert a character to lower case**

Character.toLowerCase(char)


**get a character from string s**
s.charAt(index)  

**convert string to char array**
char[] charArray = string.toCharArray();

String.split(String regex)
splits a string into an array of substrings based on the specified regular expression. 
String[] words = String.split(" ")
String[] words = String.split(" +")
split a string by one or more spaces

String.trim()
emoves leading and trailing whitespace from a string

StringBuilder vs StringBuffer


char[] charArray = word.toCharArray();
Arrays.sort(charArray);
String sortedWord = new String(charArray);


4#neet
i=0, j=1
int length = Integer.parseInt(str.substring(i,j));
