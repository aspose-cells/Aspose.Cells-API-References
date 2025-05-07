---
title: WorksheetCollection.Clear
second_title: Aspose.Cells for .NET API Reference
description: WorksheetCollection method. Clear all worksheets
type: docs
url: /net/aspose.cells/worksheetcollection/clear/
---
## WorksheetCollection.Clear method

Clear all worksheets.

```csharp
public void Clear()
```

### Remarks

A workbook must contains a worksheet.

### Examples

```csharp
// Called: pitchWorkBook.Worksheets.Clear();
[Test]
        public void Method_Clear()
        {

            Workbook pitchWorkBook = new Workbook();

            if (pitchWorkBook.Worksheets != null && pitchWorkBook.Worksheets.Count > 0)
            {
                pitchWorkBook.Worksheets.Clear();
            }

            Workbook templateWB = new Workbook(Constants.sourcePath + "CELLSNET-46196.xlsx");
            //pitchWorkBook.Copy(templateWB);
            //pitchWorkBook.CopyTheme(templateWB);
            pitchWorkBook.Combine(templateWB);
            Assert.AreEqual(259,templateWB.Worksheets[0].Shapes[0].Height);
            pitchWorkBook.Save(Constants.destPath + "CELLSNET46196.xlsx", SaveFormat.Xlsx);
        }
```

### See Also

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


