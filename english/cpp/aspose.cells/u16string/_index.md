---
title: Aspose::Cells::U16String class
linktitle: U16String
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::U16String class. Represents the char16_t array class and ends with u''\0'' in C++.'
type: docs
weight: 15600
url: /cpp/aspose.cells/u16string/
---
## U16String class


Represents the char16_t array class and ends with u'\0'.

```cpp
class U16String
```

## Methods

| Method | Description |
| --- | --- |
| [CompareTo(const U16String\& value)](./compareto/) const | Compares this instance with a specified string object. |
| [CompareTo(const U16String\& value, bool ignoreCase)](./compareto/) const | Compares this instance with a specified string object, ignoring or honoring their case. |
| [EndsWith(const U16String\& value)](./endswith/) const | Determines whether the end of this string instance matches the specified string. |
| [EndsWith(const U16String\& value, bool ignoreCase)](./endswith/) const | Determines whether the end of this string instance matches the specified string, ignoring or honoring their case. |
| [GetData()](./getdata/) const | Gets the address of the char16_t array in this vector. |
| [GetLength()](./getlength/) const | Gets the length of the char16_t array in this [Vector](../vector/). Excluding the trailing u'\0'. |
| [IndexOf(const char16_t value)](./indexof/) const | Returns the index of the first occurrence of the value in this. |
| [IndexOf(const char16_t value, int32_t startIndex)](./indexof/) const | Returns the index of the first occurrence of the value in this. |
| [IndexOf(const char16_t value, int32_t startIndex, int32_t count)](./indexof/) const | Returns the index of the first occurrence of the value in this. |
| [IndexOf(const char16_t* value)](./indexof/) const | Returns the index of the first occurrence of the value in this. |
| [IndexOf(const U16String\& value)](./indexof/) const | Returns the index of the first occurrence of the value in this. |
| [IndexOf(const U16String\& value, int32_t startIndex)](./indexof/) const | Returns the index of the first occurrence of the value in this. |
| [IndexOf(const U16String\& value, int32_t startIndex, int32_t count)](./indexof/) const | Returns the index of the first occurrence of the value in this. |
| [IndexOf(const U16String\& value, bool ignoreCase)](./indexof/) const | Returns the index of the first occurrence of the value in this. |
| [IndexOf(const U16String\& value, int32_t startIndex, int32_t count, bool ignoreCase)](./indexof/) const | Returns the index of the first occurrence of the value in this. |
| [IndexOfAny(const Vector \<char16_t\>\& anyOf)](./indexofany/) const | Reports the zero-based index of the first occurrence in this instance of any character in a specified array of characters. |
| [IndexOfAny(const Vector \<char16_t\>\& anyOf, int32_t startIndex)](./indexofany/) const | Reports the zero-based index of the first occurrence in this instance of any character in a specified array of characters. |
| [IndexOfAny(const Vector \<char16_t\>\& anyOf, int32_t startIndex, int32_t count)](./indexofany/) const | Reports the zero-based index of the first occurrence in this instance of any character in a specified array of characters. |
| [Insert(int32_t startIndex, const U16String\& str)](./insert/) const | Returns a new string in which a specified string is inserted at a specified index position in this instance. |
| [IsEmpty()](./isempty/) const | Checks whether the char16_t array is empty. |
| [IsNull()](./isnull/) const | Checks whether the object array is nullptr. |
| [LastIndexOf(const char16_t value)](./lastindexof/) const | Returns the index of the last occurrence of the value in this. |
| [LastIndexOf(const char16_t value, int32_t startIndex)](./lastindexof/) const | Returns the index of the last occurrence of the value in this. |
| [LastIndexOf(const char16_t value, int32_t startIndex, int32_t count)](./lastindexof/) const | Returns the index of the last occurrence of the value in this. |
| [LastIndexOf(const U16String\& value)](./lastindexof/) const | Returns the index of the last occurrence of the value in this. |
| [LastIndexOf(const U16String\& value, int32_t startIndex)](./lastindexof/) const | Returns the index of the last occurrence of the value in this. |
| [LastIndexOf(const U16String\& value, int32_t startIndex, int32_t count)](./lastindexof/) const | Returns the index of the last occurrence of the value in this. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator+=(const U16String\& str)](./operator+_asm/) | Concatenate another string into this. |
| [operator+=(const char* str)](./operator+_asm/) | Concatenate another string into this. |
| [operator+=(const char16_t* ustr)](./operator+_asm/) | Concatenate another string into this. |
| [operator+=(const char16_t ch)](./operator+_asm/) | Concatenate a char16_t character into this. |
| [operator=(const U16String\& str)](./operator_asm/) | operator= |
| [operator[](int32_t index)](./operator[]/) const | Array subscript operator. |
| [Remove(int32_t startIndex, int32_t count)](./remove/) const | Returns a new string in which a specified number of characters in the current instance beginning at a specified position have been deleted. |
| [Replace(const char16_t oldChar, const char16_t newChar)](./replace/) const | Returns a new string in which all occurrences of a specified character in this instance are replaced with another specified character. |
| [Replace(const char16_t* oldValue, const char16_t* newValue)](./replace/) const | Returns a new string in which all occurrences of a specified string in the current instance are replaced with another specified string. |
| [Replace(const U16String\& oldValue, const U16String\& newValue)](./replace/) const | Returns a new string in which all occurrences of a specified string in the current instance are replaced with another specified string. |
| [Split(const Vector \<char16_t\>\& separator)](./split/) const | Splits a string into substrings based on specified delimiting characters. |
| [Split(const Vector \<U16String\>\& separator)](./split/) const | Splits a string into substrings based on specified delimiting strings. |
| [StartsWith(const U16String\& value)](./startswith/) const | Determines whether the beginning of this string instance matches the specified string. |
| [StartsWith(const U16String\& value, bool ignoreCase)](./startswith/) const | Determines whether the beginning of this string instance matches the specified string. |
| [Substring(int32_t startIndex)](./substring/) const | Retrieves a substring from this instance. The substring starts at a specified character position and continues to the end of the string. |
| [Substring(int32_t startIndex, int32_t length)](./substring/) const | Retrieves a substring from this instance. The substring starts at a specified character position and has a specified length. |
| [ToLower()](./tolower/) const | Returns a copy of this string converted to lowercase. |
| [ToUpper()](./toupper/) const | Returns a copy of this string converted to uppercase. |
| [ToUtf8(char* output, int32_t len)](./toutf8/) const | Converts this to UTF8 string. |
| [ToUtf8()](./toutf8/) const | Converts this to std::string in UTF8 format. The result does not end with '\0'. |
| [Trim()](./trim/) const | Removes all leading and trailing white-space characters from the current string. |
| [Trim(char16_t trimChar)](./trim/) const | Removes all leading and trailing instances of a character from the current string. |
| [Trim(const Vector \<char16_t\>\& trimChars)](./trim/) const | Removes all leading and trailing occurrences of a set of characters specified in an array from the current string. |
| [U16String()](./u16string/) | Default constructor. Constructs an empty [U16String](./) object. |
| [U16String(const char* str)](./u16string/) | Constructs from a const char* string. |
| [U16String(const char16_t* ustr)](./u16string/) | Constructs from a const char16_t* string. |
| [U16String(const char16_t* ustr, int32_t len)](./u16string/) | Constructs from a const char16_t* string with specified length. |
| [U16String(const U16String\& src)](./u16string/) | Copy constructor. |
| [~U16String()](./~u16string/) | Destructor. |
## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
