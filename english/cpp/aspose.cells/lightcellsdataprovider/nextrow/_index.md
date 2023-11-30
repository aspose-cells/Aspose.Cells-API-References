---
title: Aspose::Cells::LightCellsDataProvider::NextRow method
linktitle: NextRow
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::LightCellsDataProvider::NextRow method. Gets the next row to be saved in C++.'
type: docs
weight: 200
url: /cpp/aspose.cells/lightcellsdataprovider/nextrow/
---
## LightCellsDataProvider::NextRow method


Gets the next row to be saved.

```cpp
virtual int32_t Aspose::Cells::LightCellsDataProvider::NextRow()=0
```


## ReturnValue

the next row index to be saved. -1 means the end of current sheet data has been reached and no further row of current sheet to be saved.
## Remarks


It will be called at the beginning of saving a row and its cells data(before StartRow(Row)). 

## See Also

* Class [Vector](../../vector/)
* Class [LightCellsDataProvider](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
