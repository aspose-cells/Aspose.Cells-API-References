---
title: Aspose::Cells::PageSetup::GetPrintTitleRows method
linktitle: GetPrintTitleRows
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PageSetup::GetPrintTitleRows method. Represents the rows that contain the cells to be repeated at the top of each page in C++.'
type: docs
weight: 1200
url: /cpp/aspose.cells/pagesetup/getprinttitlerows/
---
## PageSetup::GetPrintTitleRows method


Represents the rows that contain the cells to be repeated at the top of each page.

```cpp
U16String Aspose::Cells::PageSetup::GetPrintTitleRows()
```


## Examples


```cpp
if (pageSetup.GetPrintTitleRows().IsNull())
{
    pageSetup.SetPrintTitleRows(u"$1:$1");
}
```

## See Also

* Class [U16String](../../u16string/)
* Class [PageSetup](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
