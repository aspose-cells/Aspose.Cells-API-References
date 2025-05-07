---
title: Worksheet.Slicers
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Get the Slicer collection in the worksheet
type: docs
url: /net/aspose.cells/worksheet/slicers/
---
## Worksheet.Slicers property

Get the Slicer collection in the worksheet

```csharp
public SlicerCollection Slicers { get; }
```

### Examples

```csharp
// Called: sheet.Slicers.Add(listObject, listObject.ListColumns[2], "E16");
[Test]
        public void Property_Slicers()
        {
            string filePath = Constants.PivotTableSourcePath + @"NET47524_";
            string savePath = CreateFolder(filePath);

            Workbook wb = new Workbook(filePath + "Table.xlsx");
            Worksheet sheet = wb.Worksheets[0];
            ListObject listObject = sheet.ListObjects[0];

            sheet.Slicers.Add(listObject, listObject.ListColumns[0], 7, 8);
            sheet.Slicers.Add(listObject, 1, "B11");
            sheet.Slicers.Add(listObject, listObject.ListColumns[2], "E16");
            Assert.AreEqual(sheet.Slicers.Count, 3);
            wb.Save(savePath + "out.xlsx");
            wb.Save(savePath + "out.xlsb");

            Workbook wb2 = new Workbook(savePath + "out.xlsx");
            Assert.AreEqual(wb2.Worksheets[0].Slicers.Count, 3);
        }
```

### See Also

* class [SlicerCollection](../../../aspose.cells.slicers/slicercollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


