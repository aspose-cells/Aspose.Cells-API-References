---
title: HeaderFooterCommand.Text
second_title: Aspose.Cells for .NET API Reference
description: HeaderFooterCommand property. Gets the text of the command
type: docs
url: /net/aspose.cells/headerfootercommand/text/
---
## HeaderFooterCommand.Text property

Gets the text of the command.

```csharp
public string Text { get; }
```

### Remarks

Only valid for HeaderFooterCommandType.Text.

### Examples

```csharp
// Called: Assert.AreEqual(hfcs[1].Text, &amp;quot;sdfsdfsdfsdf&amp;quot;);
[Test]
        public void Property_Text()
        {
            Workbook workbook = new Workbook(Constants.sourcePath +&quot;CELLSJAVA40255.xlsx&quot;);
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            HeaderFooterCommand[] hfcs = ps.GetCommands(ps.GetHeader(1));

            Assert.AreEqual(hfcs[0].Type, HeaderFooterCommandType.CurrentDate);
            Assert.AreEqual(hfcs[1].Type, HeaderFooterCommandType.Text);
            Assert.AreEqual(hfcs[1].Text, &quot;sdfsdfsdfsdf&quot;);
        }
```

### See Also

* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


