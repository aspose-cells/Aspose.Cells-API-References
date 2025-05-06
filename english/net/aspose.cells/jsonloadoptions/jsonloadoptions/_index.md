---
title: JsonLoadOptions.JsonLoadOptions
second_title: Aspose.Cells for .NET API Reference
description: JsonLoadOptions constructor. Creates an options of loading the file
type: docs
url: /net/aspose.cells/jsonloadoptions/jsonloadoptions/
---
## JsonLoadOptions constructor

Creates an options of loading the file.

```csharp
public JsonLoadOptions()
```

### Examples

```csharp
// Called: JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
[Test]
        public void JsonLoadOptions_Constructor()
        {
            JsonLoadOptions options = new JsonLoadOptions { MultipleWorksheets = true };
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;NET49651.json&quot;, options);            
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;A1&quot;].StringValue, &quot;City&quot;);
            Assert.AreEqual(workbook.Worksheets[1].Cells[&quot;A1&quot;].StringValue, &quot;City2&quot;);
            Assert.AreEqual(workbook.Worksheets[2].Cells[&quot;A1&quot;].StringValue, &quot;City3&quot;);
            workbook.Save(Constants.destPath + &quot;NET49651_multisheets.xlsx&quot;);

            workbook = new Workbook(Constants.sourcePath + &quot;brateevo.json&quot;, options);

            Cells cells = workbook.Worksheets[0].Cells;
            Assert.AreEqual(cells[&quot;D5&quot;].StringValue, &quot;10к1&quot;);
            Assert.AreEqual(cells[&quot;D28&quot;].StringValue, &quot;11к1&quot;);
            Assert.AreEqual(cells[&quot;E16&quot;].StringValue, &quot;4&quot;);
            workbook.Save(Constants.destPath + &quot;NET49861_out.xlsx&quot;);

        }
```

### See Also

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


