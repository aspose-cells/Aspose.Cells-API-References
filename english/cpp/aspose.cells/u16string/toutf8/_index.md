---
title: Aspose::Cells::U16String::ToUtf8 method
linktitle: ToUtf8
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::U16String::ToUtf8 method. Converts this to UTF8 string in C++.'
type: docs
weight: 2500
url: /cpp/aspose.cells/u16string/toutf8/
---
## U16String::ToUtf8(char*, int32_t) const method


Converts this to UTF8 string.

```cpp
int32_t Aspose::Cells::U16String::ToUtf8(char *output, int32_t len) const
```


| Parameter | Type | Description |
| --- | --- | --- |
| output | char* | The output buffer. The output does not end with '\0'. |
| len | int32_t | The length of output buffer. |

## ReturnValue

The length of output buffer. If ToUtf8(nullptr, 0) is called, it returns the desired output buffer length.

## See Also

* Class [Vector](../../vector/)
* Class [U16String](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## U16String::ToUtf8() const method


Converts this to std::string in UTF8 format. The result does not end with '\0'.

```cpp
std::string Aspose::Cells::U16String::ToUtf8() const
```

## See Also

* Class [U16String](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
