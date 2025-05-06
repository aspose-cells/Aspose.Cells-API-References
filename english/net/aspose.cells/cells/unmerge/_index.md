---
title: Cells.UnMerge
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Unmerges a specified range of merged cells
type: docs
url: /net/aspose.cells/cells/unmerge/
---
## Cells.UnMerge method

Unmerges a specified range of merged cells.

```csharp
public void UnMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of this range(zero based) |
| firstColumn | Int32 | First column of this range(zero based) |
| totalRows | Int32 | Number of rows(one based) |
| totalColumns | Int32 | Number of columns(one based) |

### Examples

```csharp
// Called: cells.UnMerge(0, 0, 65536, 256);
[Test]
        public void Method_Int32_()
        {
            caseName = &quot;testUnMerge_002&quot;;
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Cells\\cellsMerge_002.xls&quot;);
            Cells cells = workbook.Worksheets[0].Cells;
            cells.UnMerge(0, 0, 65536, 256);

            checkUnMerge_001(workbook);
            workbook.Save(Constants.destPath + &quot; testStandardWidth.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot; testStandardWidth.xls&quot;);
            checkUnMerge_001(workbook);
            workbook.Save(Constants.destPath + &quot; testStandardWidth.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot; testStandardWidth.xlsx&quot;);
            checkUnMerge_001(workbook);
            workbook.Save(Constants.destPath + &quot; testStandardWidth.xml&quot;, SaveFormat.SpreadsheetML);
            workbook = new Workbook(Constants.destPath + &quot; testStandardWidth.xml&quot;);
            checkUnMerge_001(workbook);
            workbook.Save(Constants.destPath + &quot; testStandardWidth.xls&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


