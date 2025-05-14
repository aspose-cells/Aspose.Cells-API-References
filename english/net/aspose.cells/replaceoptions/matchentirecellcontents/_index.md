---
title: ReplaceOptions.MatchEntireCellContents
second_title: Aspose.Cells for .NET API Reference
description: ReplaceOptions property. Indicates whether to match entire cells contents
type: docs
url: /net/aspose.cells/replaceoptions/matchentirecellcontents/
---
## ReplaceOptions.MatchEntireCellContents property

Indicates whether to match entire cells contents

```csharp
public bool MatchEntireCellContents { get; set; }
```

### Remarks

The default value is true.

### Examples

```csharp
// Called: replace.MatchEntireCellContents = false;
public void ReplaceOptions_Property_MatchEntireCellContents()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    ReplaceOptions replace = new ReplaceOptions();
    replace.CaseSensitive = false;
    replace.MatchEntireCellContents = false;
    workbook.Replace("[b_phone]", "123123123", replace);
    Assert.AreEqual(workbook.Worksheets[0].Cells["A4"].StringValue, "phone 123123123 ");
}
```

### See Also

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


