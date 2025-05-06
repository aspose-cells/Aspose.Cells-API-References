---
title: HeaderFooterCommand.Type
second_title: Aspose.Cells for .NET API Reference
description: HeaderFooterCommand property. Gets the header/footer command type 
type: docs
url: /net/aspose.cells/headerfootercommand/type/
---
## HeaderFooterCommand.Type property

Gets the header/footer' command type .

```csharp
public HeaderFooterCommandType Type { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(hfcs[0].Type, HeaderFooterCommandType.CurrentDate);
[Test]
        public void Property_Type()
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

* enum [HeaderFooterCommandType](../../headerfootercommandtype/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


