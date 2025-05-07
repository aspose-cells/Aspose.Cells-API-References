---
title: Cell.Copy
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Copies data from a source cell
type: docs
url: /net/aspose.cells/cell/copy/
---
## Cell.Copy method

Copies data from a source cell.

```csharp
public void Copy(Cell cell)
```

| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | Source [`Cell`](../) object. |

### Examples

```csharp
// Called: cells[0, 2].Copy(cells[0, 0]);
[Test]
        public void Method_Cell_()
        {
            caseName = "testCopy_002";
            Workbook workbook = new Workbook(Constants.sourcePath + "Cells\\copy_001.xls");
            Cells cells = workbook.Worksheets[0].Cells;
            cells[0, 2].Copy(cells[0, 0]);
            cells[1, 2].Copy(cells[1, 0]);
            cells[2, 2].Copy(cells[2, 0]);
            cells[3, 2].Copy(cells[3, 0]);

            workbook.Save(Constants.destPath + "testCopy.xls");            
            workbook = new Workbook(Constants.destPath + "testCopy.xls");
            checkCopy_001(workbook);
            workbook.Save(Constants.destPath + "testCopy.xlsx");            
            workbook = new Workbook(Constants.destPath + "testCopy.xlsx");
            checkCopy_001(workbook);
            workbook.Save(Constants.destPath + "testCopy.xml", SaveFormat.SpreadsheetML);            
            workbook = new Workbook(Constants.destPath + "testCopy.xml");
            checkCopy_001(workbook);
            workbook.Save(Constants.destPath + "testCopy.xls"); 
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


