---
title: Class HeaderFooterCommand
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.HeaderFooterCommand class. Represents the command of header/footer
type: docs
url: /net/aspose.cells/headerfootercommand/
---
## HeaderFooterCommand class

Represents the command of header/footer

```csharp
public class HeaderFooterCommand
```

## Properties

| Name | Description |
| --- | --- |
| [Font](../../aspose.cells/headerfootercommand/font/) { get; } | Gets the font of the command's value. |
| [Text](../../aspose.cells/headerfootercommand/text/) { get; } | Gets the text of the command. |
| [Type](../../aspose.cells/headerfootercommand/type/) { get; } | Gets the header/footer' command type . |

### Examples

```csharp
// Called: HeaderFooterCommand[] hfcs = ps.GetCommands(ps.GetHeader(1));
public void Cells_Type_HeaderFooterCommand()
{
    Workbook workbook = new Workbook(Constants.sourcePath +"example.xlsx");
    PageSetup ps = workbook.Worksheets[0].PageSetup;
    HeaderFooterCommand[] hfcs = ps.GetCommands(ps.GetHeader(1));

    Assert.AreEqual(hfcs[0].Type, HeaderFooterCommandType.CurrentDate);
    Assert.AreEqual(hfcs[1].Type, HeaderFooterCommandType.Text);
    Assert.AreEqual(hfcs[1].Text, "sdfsdfsdfsdf");
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


