---
title: WorksheetCollection.OleSize
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection property. Gets and Sets displayed size when Workbook file is used as an Ole object
type: docs
url: /net/aspose.cells/worksheetcollection/olesize/
---
## WorksheetCollection.OleSize property

Gets and Sets displayed size when Workbook file is used as an Ole object.

```csharp
public object OleSize { get; set; }
```

### Remarks

Null means no ole size setting.

### Examples

```csharp
// Called: Assert.AreEqual(((CellArea)workbook.Worksheets.OleSize).EndRow, 10);
[Test]
        public void Property_OleSize()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.SetOleSize(0, 10, 0, 10);
            workbook.Save(Constants.destPath + "CELLSJAVA40634.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSJAVA40634.xlsx");
            Assert.AreEqual(((CellArea)workbook.Worksheets.OleSize).EndRow, 10);
            workbook.Save(Constants.destPath + "CELLSJAVA40634.xls");
            workbook = new Workbook(Constants.destPath + "CELLSJAVA40634.xls");
            Assert.AreEqual(((CellArea)workbook.Worksheets.OleSize).EndRow, 10);

        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


