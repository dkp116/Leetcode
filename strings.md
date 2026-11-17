## Strings 

### Useful functions

    to_string converts a number to stirng 
    stio converts string to integer
    
    To convert characters to numbers: 
    char - '0'

    To convert numbers to char:
    stio ? 

    Get substring 
    s.substr(position you want to start , size of the substring)

    If you have a sentence with spaces consider using sstream 
    ssteam stream(the string sentence)

    To extract out each word
    while(string example << stream){
        example - is the word 
    }

    You can also split by delminater

    use while(getline(string stream, example , ' delminater')){
        example is now each string before the delminater
    }
