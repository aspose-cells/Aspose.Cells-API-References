---
title: PageSetup.GetHeader
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Gets a script formatting the header of an Excel file
type: docs
url: /net/aspose.cells/pagesetup/getheader/
---
## PageSetup.GetHeader method

Gets a script formatting the header of an Excel file.

```csharp
public string GetHeader(int section)
```

| Parameter | Type | Description |
| --- | --- | --- |
| section | Int32 | 0: Left Section, 1: Center Section, 2: Right Section. |

### Examples

```csharp
// Called: HeaderFooterCommand[] hfcs = ps.GetCommands(ps.GetHeader(1));
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath +"CELLSJAVA40255.xlsx");
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            HeaderFooterCommand[] hfcs = ps.GetCommands(ps.GetHeader(1));

            Assert.AreEqual(hfcs[0].Type, HeaderFooterCommandType.CurrentDate);
            Assert.AreEqual(hfcs[1].Type, HeaderFooterCommandType.Text);
            Assert.AreEqual(hfcs[1].Text, "sdfsdfsdfsdf");
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


