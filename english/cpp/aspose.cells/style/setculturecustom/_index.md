﻿---
title: Aspose::Cells::Style::SetCultureCustom method
linktitle: SetCultureCustom
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Style::SetCultureCustom method. Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned in C++.'
type: docs
weight: 6200
url: /cpp/aspose.cells/style/setculturecustom/
---
## Style::SetCultureCustom(const U16String\&) method


Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.

```cpp
void Aspose::Cells::Style::SetCultureCustom(const U16String &value)
```

## Remarks


For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales, but for some other locales it becomes "d/m/y") and the format specifier(such as, some locales is using character other than 'y' to represent the year part for date formatting) are culture-dependent; For user specified custom format, only format specifiers are changed according to the culture, other parts of the formatting pattern will not be modified. 
## See Also

* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Style](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Style::SetCultureCustom(const char16_t*) method


Gets and sets the culture-dependent pattern string for number format. If no number format has been set for this object, null will be returned. If number format is builtin, the pattern string corresponding to the builtin number will be returned.

```cpp
void Aspose::Cells::Style::SetCultureCustom(const char16_t *value)
```

## Remarks


For builtin number format, both the pattern content(such as, one builtin date format is "m/d/y" for some locales, but for some other locales it becomes "d/m/y") and the format specifier(such as, some locales is using character other than 'y' to represent the year part for date formatting) are culture-dependent; For user specified custom format, only format specifiers are changed according to the culture, other parts of the formatting pattern will not be modified. 
## See Also

* Class [Vector](../../vector/)
* Class [Style](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
