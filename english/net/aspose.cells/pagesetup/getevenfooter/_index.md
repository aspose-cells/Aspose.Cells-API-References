---
title: PageSetup.GetEvenFooter
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Gets a script formatting the even footer of an Excel file
type: docs
url: /net/aspose.cells/pagesetup/getevenfooter/
---
## PageSetup.GetEvenFooter method

Gets a script formatting the even footer of an Excel file.

```csharp
public string GetEvenFooter(int section)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].PageSetup.GetEvenFooter(1), "even");
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet23659.xls");
            Assert.AreEqual(workbook.Worksheets[0].PageSetup.GetFirstPageFooter(1), "first");
            Assert.AreEqual(workbook.Worksheets[0].PageSetup.GetEvenFooter(1), "even");
            Assert.AreEqual(workbook.Worksheets[0].PageSetup.GetFooter(1), "odd");
            workbook.Save(Constants.destPath + "CellsNet23659.xls");
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


