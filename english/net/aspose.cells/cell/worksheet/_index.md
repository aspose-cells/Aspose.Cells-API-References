---
title: Cell.Worksheet
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the parent worksheet
type: docs
url: /net/aspose.cells/cell/worksheet/
---
## Cell.Worksheet property

Gets the parent worksheet.

```csharp
public Worksheet Worksheet { get; }
```

### Examples

```csharp
// Called: cell.Worksheet.Cells.DeleteColumns(cell.Column + 1, 8, true);
[Test]
       public void Property_Worksheet()
       {
           var book = new Workbook(Constants.sourcePath + "CellsNet43338.xlt");
           //var book = new Workbook(@".\test11.xltx"); 

           var cell = book.Worksheets[0].Cells[4, 8];

           const int colsToInsert = 20;
           //const int colsToInsert = 5; 

           // delete all columns in region that will be expanded except for first and last 
           cell.Worksheet.Cells.DeleteColumns(cell.Column + 1, 8, true);
           // insert columns between first and last to make table expand 
           cell.Worksheet.Cells.InsertColumns(cell.Column + 1, colsToInsert, true);
           // delete last column 
           cell.Worksheet.Cells.DeleteColumn(cell.Column + 1 + colsToInsert);
           Assert.AreEqual(cell.Worksheet.Cells["A4"].StringValue, "Char.\nNumber");
       }
```

### See Also

* class [Worksheet](../../worksheet/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


