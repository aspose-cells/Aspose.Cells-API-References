---
title: JsonLoadOptions.MultipleWorksheets
second_title: Aspose.Cells for .NET API Reference
description: JsonLoadOptions property. Indicates whether importing each attribute of JsonObject object as one worksheet when all child nodes are array nodes
type: docs
url: /net/aspose.cells/jsonloadoptions/multipleworksheets/
---
## JsonLoadOptions.MultipleWorksheets property

Indicates whether importing each attribute of JsonObject object as one worksheet when all child nodes are array nodes.

```csharp
public bool MultipleWorksheets { get; set; }
```

### Examples

```csharp
// Called: JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
[Test]
        public void Property_MultipleWorksheets()
        {
            JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSAPP1303.json&quot;, options);
            Cells cells = wb.Worksheets[0].Cells;
            Assert.AreEqual(cells[&quot;D5&quot;].StringValue, &quot;t&quot;);
            Assert.AreEqual(cells[&quot;E5&quot;].StringValue, &quot;c&quot;);
            Assert.AreEqual(cells[&quot;D7&quot;].StringValue, &quot;underline&quot;);
            Assert.AreEqual(cells[&quot;B14&quot;].StringValue, &quot;1&quot;);

        }
```

### See Also

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


