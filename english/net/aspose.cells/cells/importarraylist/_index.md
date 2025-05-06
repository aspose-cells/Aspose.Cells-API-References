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
// Called: cells.ImportArrayList(list, 1048575, 0, false);
[Test]
        public void Method_Boolean_()
        {
            caseName = &quot;testImportArrayList_Excel2007_002&quot;;
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            ArrayList list = new ArrayList();
            list.Add(10);
            list.Add(true);
            list.Add(-0.86);
            list.Add(&quot;abc&quot;);
            cells.ImportArrayList(list, 1048575, 0, false);

            checkImportArrayList_Excel2007_002(workbook, list);
            workbook.Save(Constants.destPath + &quot;testImportArrayList.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testImportArrayList.xlsx&quot;);
            checkImportArrayList_Excel2007_002(workbook, list);
            workbook.Save(Constants.destPath + &quot;testImportArrayList.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot;testImportArrayList.xml&quot;);
            workbook.Save(Constants.destPath + &quot;testImportArrayList.xls&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


