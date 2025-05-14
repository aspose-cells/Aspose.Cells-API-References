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
public void JsonLoadOptions_Property_MultipleWorksheets()
{
    JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
    Workbook wb = new Workbook(Constants.sourcePath + "example.json", options);
    Cells cells = wb.Worksheets[0].Cells;
    Assert.AreEqual(cells["D5"].StringValue, "t");
    Assert.AreEqual(cells["E5"].StringValue, "c");
    Assert.AreEqual(cells["D7"].StringValue, "underline");
    Assert.AreEqual(cells["B14"].StringValue, "1");

}
```

### See Also

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


