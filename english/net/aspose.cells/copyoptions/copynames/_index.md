---
title: CopyOptions.CopyNames
second_title: Aspose.Cells for .NET API Reference
description: CopyOptions property. Indicates whether copying the names
type: docs
url: /net/aspose.cells/copyoptions/copynames/
---
## CopyOptions.CopyNames property

Indicates whether copying the names.

```csharp
public bool CopyNames { get; set; }
```

### Examples

```csharp
// Called: newWorkbook.Worksheets[0].Copy(workbook.Worksheets["Sheet1"], new CopyOptions { CopyNames = true });
[Test]
        public void Property_CopyNames()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET-43083_1.xlsx");
            Workbook newWorkbook = new Workbook();
            newWorkbook.Worksheets[0].Copy(workbook.Worksheets["Sheet1"], new CopyOptions { CopyNames = true });
            string f = newWorkbook.Worksheets[0].Cells["D10"].Formula;
            Assert.AreEqual(f, "=Name3");
            string expected = "[CELLSNET-43083_1.xlsx]Sheet2'!$C$2";
            string act = newWorkbook.Worksheets.Names["Name3"].RefersTo;
            if (!act.EndsWith(expected))
            {
                Assert.Fail("Name3.RefersTo should end with " + expected + " but was " + act);
            }
            workbook = new Workbook(Constants.sourcePath + "CELLSNET-43083_2.xlsx");
            newWorkbook = new Workbook();
            newWorkbook.Worksheets[0].Copy(workbook.Worksheets["Sheet1"], new CopyOptions { CopyNames = true });
            expected = "Another book.xlsx'!Name6";
            act = newWorkbook.Worksheets[0].Cells["D11"].Formula;
            if (!act.EndsWith(expected))
            {
                Assert.Fail("D11.Formula should end with " + expected + " but was " + act);
            }
            expected = "CELLSNET-43083_2.xlsx'!Table1)";
            act = newWorkbook.Worksheets[0].Cells["D12"].Formula;
            if (!act.EndsWith(expected))
            {
                Assert.Fail("D12.Formula should end with " + expected + " but was " + act);
            }
        }
```

### See Also

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


