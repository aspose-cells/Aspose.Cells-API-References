---
title: CopyOptions.CopyOptions
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions constructor. CopyOptions constructor
type: docs
url: /net/aspose.cells/copyoptions/copyoptions/
---
## CopyOptions constructor

CopyOptions constructor.

```csharp
public CopyOptions()
```

### Examples

```csharp
// Called: Aspose.Cells.CopyOptions options = new Aspose.Cells.CopyOptions();
[Test]
        public void CopyOptions_Constructor()
        {
            string templetePath = Constants.sourcePath + "CellsNet44203.xlsx";
            Workbook templeteWorkbook = new Aspose.Cells.Workbook(templetePath);
            Workbook outputWorkbook = new Aspose.Cells.Workbook();

            for (int i = 0; i < templeteWorkbook.Worksheets.Count; i++)
            {
                outputWorkbook.Worksheets.Add(templeteWorkbook.Worksheets[i].Name);
            }
            for (int i = 0; i < templeteWorkbook.Worksheets.Count; i++)
            {
                Aspose.Cells.CopyOptions options = new Aspose.Cells.CopyOptions();
                options.ReferToSheetWithSameName = true;
                outputWorkbook.Worksheets[templeteWorkbook.Worksheets[i].Name].Copy(templeteWorkbook.Worksheets[i]);
            }

            outputWorkbook.Worksheets.RemoveAt(0);
            outputWorkbook.Worksheets.RemoveAt("Start");
            outputWorkbook.Worksheets.RemoveAt("End");
            Assert.AreEqual("=SUM(Detail!B3)", outputWorkbook.Worksheets[0].Cells["B3"].Formula);
        }
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


