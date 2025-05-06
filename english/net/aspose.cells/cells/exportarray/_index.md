---
title: Cells.ExportArray
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Exports data in the Cells collection to a twodimension array object
type: docs
url: /net/aspose.cells/cells/exportarray/
---
## Cells.ExportArray method

Exports data in the [`Cells`](../) collection to a two-dimension array object.

```csharp
public object[] ExportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | The row number of the first cell to export out. |
| firstColumn | Int32 | The column number of the first cell to export out. |
| totalRows | Int32 | Number of rows to be exported |
| totalColumns | Int32 | Number of columns to be exported |

### Return Value

Exported cell value array object.

### Examples

```csharp
// Called: Object[,] objarr  = cells.ExportArray(65531, 0, 5, 2);
[Test]
        public void Method_Int32_()
        {
            caseName = &quot;testExportArray_004&quot;;
            Workbook workbook = new Workbook();            
            workbook = new Workbook(Constants.sourcePath + &quot;Cells\\exportArray_002.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            Object[,] objarr  = cells.ExportArray(65531, 0, 5, 2);

            checkExportArray_003(workbook, objarr);
            workbook.Save(Constants.destPath + &quot;testExportArray.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testExportArray.xls&quot;);
            checkExportArray_003(workbook, objarr);
            workbook.Save(Constants.destPath + &quot;testExportArray.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;testExportArray.xlsx&quot;);
            checkExportArray_003(workbook, objarr);
            workbook.Save(Constants.destPath + &quot;testExportArray.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot;testExportArray.xml&quot;);
            checkExportArray_003(workbook, objarr);
            workbook.Save(Constants.destPath + &quot;testExportArray.xls&quot;); 
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


