---
title: Aspose::Cells::Color::FromName method
linktitle: FromName
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Color::FromName method. Creates a Color from a predefined color name in C++.'
type: docs
weight: 400
url: /cpp/aspose.cells/color/fromname/
---
## Color::FromName method


Creates a [Color](../) from a predefined color name.

```cpp
static Color Aspose::Cells::Color::FromName(const U16String &name)
```


| Parameter | Type | Description |
| --- | --- | --- |
| name | const U16String\& | A UTF-16 string containing the name of the color. The comparison is case-insensitive. |

## ReturnValue

A [Color](../) structure that corresponds to the specified name.
## Remarks



Supports the standard set of 174 HTML color names (CSS named colors), such as **red**, **green**, **blue**, **black**, and **white**. 

## Examples


```cpp
auto red   = Color::FromName(u"red");
auto blue  = Color::FromName(u"Blue");
auto white = Color::FromName(u"WHITE");
```

## See Also

* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
