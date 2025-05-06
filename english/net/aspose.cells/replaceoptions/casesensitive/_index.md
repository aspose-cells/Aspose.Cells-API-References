---
title: ReplaceOptions.CaseSensitive
second_title: Aspose.Cells for .NET API Reference
description: ReplaceOptions property. Indicates if the searched string is case sensitive
type: docs
url: /net/aspose.cells/replaceoptions/casesensitive/
---
## ReplaceOptions.CaseSensitive property

Indicates if the searched string is case sensitive.

```csharp
public bool CaseSensitive { get; set; }
```

### Examples

```csharp
// Called: replace.CaseSensitive = false;
[Test]
        public void Property_CaseSensitive()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet_12489.xls&quot;);
            ReplaceOptions replace = new ReplaceOptions();
            replace.CaseSensitive = false;
            replace.MatchEntireCellContents = false;
            workbook.Replace(&quot;[b_phone]&quot;, &quot;123123123&quot;, replace);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;A4&quot;].StringValue, &quot;phone 123123123 &quot;);
        }
```

### See Also

* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


