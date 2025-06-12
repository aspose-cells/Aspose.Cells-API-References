---
title: Aspose::Cells::ReferredArea::GetValues method
linktitle: GetValues
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::ReferredArea::GetValues method. Gets cell values in this area in C++.'
type: docs
weight: 1700
url: /cpp/aspose.cells/referredarea/getvalues/
---
## ReferredArea::GetValues() method


Gets cell values in this area.

```cpp
Aspose::Cells::Object Aspose::Cells::ReferredArea::GetValues()
```


## ReturnValue

If this area is invalid, "#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.

## See Also

* Class [Object](../../object/)
* Class [ReferredArea](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## ReferredArea::GetValues(bool) method


Gets cell values in this area.

```cpp
Aspose::Cells::Object Aspose::Cells::ReferredArea::GetValues(bool calculateFormulas)
```


| Parameter | Type | Description |
| --- | --- | --- |
| calculateFormulas | bool | In this range, if there are some formulas that have not been calculated, this flag denotes whether those formulas should be calculated recursively |

## ReturnValue

If this area is invalid, "#REF!" will be returned; If this area is one single cell, then return the cell value object; Otherwise return one 2D array for all values in this area.

## See Also

* Class [Object](../../object/)
* Class [Vector](../../vector/)
* Class [ReferredArea](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
