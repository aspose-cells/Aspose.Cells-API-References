---
title: Aspose::Cells::WorkbookSettings::SetIsHScrollBarVisible method
linktitle: SetIsHScrollBarVisible
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::WorkbookSettings::SetIsHScrollBarVisible method. Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar in C++.'
type: docs
weight: 2600
url: /cpp/aspose.cells/workbooksettings/setishscrollbarvisible/
---
## WorkbookSettings::SetIsHScrollBarVisible method


Gets or sets a value indicating whether the generated spreadsheet will contain a horizontal scroll bar.

```cpp
void Aspose::Cells::WorkbookSettings::SetIsHScrollBarVisible(bool value)
```

## Remarks


The default value is true.

## Examples


```cpp
//The following code makes the horizontal scroll bar invisible for the spreadsheet.
// Hide the horizontal scroll bar of the Excel file.
if (settings.IsHScrollBarVisible())
{
    settings.SetIsHScrollBarVisible(false);
}
```

## See Also

* Class [Vector](../../vector/)
* Class [WorkbookSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
