---
title: Workbook.FileName
second_title: Aspose.Cells for .NET API Reference
description: Workbook property. Gets and sets the current file name
type: docs
url: /net/aspose.cells/workbook/filename/
---
## Workbook.FileName property

Gets and sets the current file name.

```csharp
public string FileName { get; set; }
```

### Remarks

If the file is opened by stream and there are some external formula references, please set the file name.

### Examples

```csharp
// Called: wb1.FileName = wb.Worksheets.ExternalLinks[0].DataSource;
private void Workbook_Property_FileName(bool link)
        {
            Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
            if (link)
            {
                Workbook wb1 = new Workbook(Constants.sourcePath + "example.xlsx");
                wb1.FileName = wb.Worksheets.ExternalLinks[0].DataSource;
                //below should work too
                //wb1.FileName = "../../../Files/template/Formula/calculate/report.xlsx";
                //wb1.FileName = "..\\..\\Files\\template\\Formula\\calculate\\report.xlsx";
                wb.UpdateLinkedDataSource(new Workbook[] { wb1 });
            }
            Cells cells = wb.Worksheets[0].Cells;
            wb.CalculateFormula();
            for (int i = 1; i < 4; i++)
            {
                Assert.AreEqual(100, cells[1, i].IntValue, ((char)('A' + i)) + "2");
            }
            for (int i = 1; i < 4; i++)
            {
                Assert.AreEqual(200, cells[2, i].IntValue, ((char)('A' + i)) + "2");
            }
        }
```

### See Also

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


