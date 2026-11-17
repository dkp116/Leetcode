
## Strings

### Useful Functions

- **`to_string()`** converts a number to a string.
- **`stoi()`** converts a string to an integer.

### Converting Characters and Numbers

To convert a character representing a digit into an integer:

```cpp
char c = '5';
int num = c - '0';
```

To convert an integer into a character representing a digit:

```cpp
int num = 5;
char c = num + '0';
```

### Getting a Substring

Use `substr()` to extract part of a string.

```cpp
s.substr(position, length);
```

- `position` – index where the substring starts.
- `length` – number of characters to extract.

### Working with Sentences and Spaces

If you have a sentence containing spaces, consider using `stringstream`.

```cpp
#include <sstream>

stringstream stream(sentence);
```

To extract each word individually:

```cpp
string example;

while (stream >> example) {
    // example contains the next word
}
```

### Splitting a String by a Delimiter

You can also split a string using a delimiter with `getline()`.

```cpp
stringstream stream(s);
string example;

while (getline(stream, example, ' ')) {
    // example contains the next part of the string
}
```

Replace `' '` with your desired delimiter (e.g. `','`, `'-'`, etc.).
