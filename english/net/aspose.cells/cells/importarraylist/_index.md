---
title: Cells.ImportArrayList
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Imports an arraylist of data into a worksheet
type: docs
url: /net/aspose.cells/cells/importarraylist/
---
## Cells.ImportArrayList method

Imports an arraylist of data into a worksheet.

```csharp
public void ImportArrayList(ArrayList arrayList, int firstRow, int firstColumn, bool isVertical)
```

| Parameter | Type | Description |
| --- | --- | --- |
| arrayList | ArrayList | Data arraylist. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| isVertical | Boolean | Specifies to import data vertically or horizontally. |

### Examples

```csharp
// Called: cells.ImportArrayList(list, 1048576, 0, true);
[Test, ExpectedException(typeof(CellsException))]
#endif
        public void Cells_Method_ImportArrayList()
        {
            caseName = "testImportArrayList_Exception_002";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            ArrayList list = new ArrayList();
            list.Add(10);
            list.Add("abc");
            list.Add(true);
            cells.ImportArrayList(list, 1048576, 0, true);
            string msg = message + "cells.ImportArrayList(list, 1048576, 0, true)";
            writeToExcel(caseName, msg);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


