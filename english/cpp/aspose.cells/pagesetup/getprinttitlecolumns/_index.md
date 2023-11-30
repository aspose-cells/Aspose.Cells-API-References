---
title: Aspose::Cells::PageSetup::GetPrintTitleColumns method
linktitle: GetPrintTitleColumns
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PageSetup::GetPrintTitleColumns method. Represents the columns that contain the cells to be repeated on the left side of each page in C++.'
type: docs
weight: 1000
url: /cpp/aspose.cells/pagesetup/getprinttitlecolumns/
---
## PageSetup::GetPrintTitleColumns method


Represents the columns that contain the cells to be repeated on the left side of each page.

```cpp
U16String Aspose::Cells::PageSetup::GetPrintTitleColumns()
```


## Examples


```cpp
if (pageSetup.GetPrintTitleColumns().IsNull())
{
    pageSetup.SetPrintTitleColumns(u"$A:$A");
}
```

## See Also

* Class [U16String](../../u16string/)
* Class [PageSetup](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
