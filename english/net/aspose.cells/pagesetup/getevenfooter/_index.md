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
// Called: Assert.AreEqual(workbook.Worksheets[0].PageSetup.GetEvenFooter(1), &amp;quot;even&amp;quot;);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet23659.xls&quot;);
            Assert.AreEqual(workbook.Worksheets[0].PageSetup.GetFirstPageFooter(1), &quot;first&quot;);
            Assert.AreEqual(workbook.Worksheets[0].PageSetup.GetEvenFooter(1), &quot;even&quot;);
            Assert.AreEqual(workbook.Worksheets[0].PageSetup.GetFooter(1), &quot;odd&quot;);
            workbook.Save(Constants.destPath + &quot;CellsNet23659.xls&quot;);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


