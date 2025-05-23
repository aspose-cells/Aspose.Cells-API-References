---
title: PageSetup.GetCommands
second_title: Aspose.Cells for .NET API Reference
description: PageSetup method. Gets all commands of header or footer
type: docs
url: /net/aspose.cells/pagesetup/getcommands/
---
## PageSetup.GetCommands method

Gets all commands of header or footer.

```csharp
public HeaderFooterCommand[] GetCommands(string headerFooterScript)
```

| Parameter | Type | Description |
| --- | --- | --- |
| headerFooterScript | String | The header/footer script |

### Return Value

Returns all commands of header or footer.

### Examples

```csharp
// Called: HeaderFooterCommand[] hfcs = ps.GetCommands(ps.GetHeader(1));
public void PageSetup_Method_GetCommands()
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

* class [HeaderFooterCommand](../../headerfootercommand/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


