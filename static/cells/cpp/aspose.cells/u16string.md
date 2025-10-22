##Aspose::Cells::U16String class
'Aspose::Cells::U16String class. Represents the char16_t array class and ends with u''\0'' in C++.'
## U16String class
Represents the char16_t array class and ends with u'\0'.
```cpp
class U16String
```
## Methods
| Method | Description |
| --- | --- |
| [GetData()](./getdata/) const | Gets the address of the char16_t array in this vector. |
| [GetLength()](./getlength/) const | Gets the length of the char16_t array in this [Vector](../vector/). Excluding the trailing u'\0'. |
| [IndexOf(const char16_t value)](./indexof/) const | Returns the index of the first occurrence of the value in this. |
| [IndexOf(const char16_t* value)](./indexof/) const | Returns the index of the first occurrence of the value in this. |
| [IndexOf(const U16String\& value)](./indexof/) const | Returns the index of the first occurrence of the value in this. |
| [IsEmpty()](./isempty/) const | Checks whether the char16_t array is empty. |
| [IsNull()](./isnull/) const | Checks whether the object array is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator+=(const U16String\& str)](./operator+_asm/) | Concatenate another string into this. |
| [operator+=(const char* str)](./operator+_asm/) | Concatenate another string into this. |
| [operator+=(const char16_t* ustr)](./operator+_asm/) | Concatenate another string into this. |
| [operator+=(const char16_t ch)](./operator+_asm/) | Concatenate a char16_t character into this. |
| [operator=(const U16String\& str)](./operator_asm/) | operator= |
| [operator[](int32_t index)](./operator[]/) | Array subscript operator. |
| [ToUtf8(char* output, int32_t len)](./toutf8/) const | Converts this to UTF8 string. |
| [ToUtf8()](./toutf8/) const | Converts this to std::string in UTF8 format. The result does not end with '\0'. |
| [Trim()](./trim/) const | Trims leading and trailing spaces in this. |
| [U16String()](./u16string/) | Default constructor. Constructs an empty [U16String](./) object. |
| [U16String(const char* str)](./u16string/) | Constructs from a const char* string. |
| [U16String(const char16_t* ustr)](./u16string/) | Constructs from a const char16_t* string. |
| [U16String(const char16_t* ustr, int32_t len)](./u16string/) | Constructs from a const char16_t* string with specified length. |
| [U16String(const U16String\& src)](./u16string/) | Copy constructor. |
| [~U16String()](./~u16string/) | Destructor. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
