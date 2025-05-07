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
// Called: cells.ImportArrayList(list, 0, 255, true);
[Test]
        public void Method_Boolean_()
        {
            caseName = "testImportArrayList_008";
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            ArrayList list = new ArrayList();
            list.Add(10);
            list.Add(true);
            list.Add(-0.86);
            list.Add("abc");
            cells.ImportArrayList(list, 0, 255, true);

            checkImportArrayList_008(workbook, list);
            workbook.Save(Constants.destPath + "testImportArrayList.xls");
            workbook = new Workbook(Constants.destPath + "testImportArrayList.xls");
            checkImportArrayList_008(workbook, list);
            workbook.Save(Constants.destPath + "testImportArrayList.xlsx");
            workbook = new Workbook(Constants.destPath + "testImportArrayList.xlsx");
            checkImportArrayList_008(workbook, list);
            workbook.Save(Constants.destPath + "testImportArrayList.xml", SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + "testImportArrayList.xml");
            checkImportArrayList_008(workbook, list);
            workbook.Save(Constants.destPath + "testImportArrayList.xls"); 
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


