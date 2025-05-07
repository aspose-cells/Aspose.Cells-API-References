---
title: Workbook.SaveToStream
second_title: Aspose.Cells for .NET API Reference
description: Workbook method. Saves Excel file to a MemoryStream object and returns it
type: docs
url: /net/aspose.cells/workbook/savetostream/
---
## Workbook.SaveToStream method

Saves Excel file to a MemoryStream object and returns it.

```csharp
public MemoryStream SaveToStream()
```

### Return Value

MemoryStream object which contains an Excel file.

### Remarks

This method provides same function as Save method and only save the workbook as Excel97-2003 xls file. It's mainly for calling from COM clients.

### Examples

```csharp
// Called: Workbook workbook = new Workbook(start.SaveToStream());
[Test]
        public void Method_SaveToStream()
        {
         //   Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet41525");
            Workbook start = new Workbook(Constants.sourcePath + "CellsNet41525.xlsx");

            Workbook workbook = new Workbook(start.SaveToStream());

            //Accessing the first worksheet in the Excel file
            Worksheet worksheet = workbook.Worksheets[0];

            var area = CellArea.CreateCellArea(3, 0, 3, 1);

            worksheet.Cells.InsertRange(area, 3, ShiftType.Down, true);

            worksheet.Cells["A4"].PutValue("D");
            worksheet.Cells["B4"].PutValue(40);

            worksheet.Cells["A5"].PutValue("E");
            worksheet.Cells["B5"].PutValue(50);

            worksheet.Cells["A6"].PutValue("F");
            worksheet.Cells["B6"].PutValue(60);


            workbook.Worksheets[0].Charts[0].Calculate();


            //Saving the modified Excel file
            Assert.AreEqual(workbook.Worksheets[1].Charts[0].NSeries[0].Values, "=Sheet1!$B$2:$B$7");

        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


