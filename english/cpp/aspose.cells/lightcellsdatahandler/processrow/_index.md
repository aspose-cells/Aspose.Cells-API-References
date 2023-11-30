---
title: Aspose::Cells::LightCellsDataHandler::ProcessRow method
linktitle: ProcessRow
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::LightCellsDataHandler::ProcessRow method. Starts to process one row in C++.'
type: docs
weight: 300
url: /cpp/aspose.cells/lightcellsdatahandler/processrow/
---
## LightCellsDataHandler::ProcessRow method


Starts to process one row.

```cpp
virtual bool Aspose::Cells::LightCellsDataHandler::ProcessRow(Row &row)=0
```


| Parameter | Type | Description |
| --- | --- | --- |
| row | Row\& | [Row](../../row/) object which is being processed currently. |

## ReturnValue

whether this row's cells need to be processed. false to ignore all cells in this row.
## Remarks


It will be called after row's properties such as height, style, ...etc. have been read. However, cells in this row has not been read yet. 

## See Also

* Class [Vector](../../vector/)
* Class [Row](../../row/)
* Class [LightCellsDataHandler](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
