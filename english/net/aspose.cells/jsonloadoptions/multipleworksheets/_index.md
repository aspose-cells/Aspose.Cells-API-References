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
            Workbook workbook = new Workbook(Constants.sourcePath + "NET49651.json", options);            
            Assert.AreEqual(workbook.Worksheets[0].Cells["A1"].StringValue, "City");
            Assert.AreEqual(workbook.Worksheets[1].Cells["A1"].StringValue, "City2");
            Assert.AreEqual(workbook.Worksheets[2].Cells["A1"].StringValue, "City3");
            workbook.Save(Constants.destPath + "NET49651_multisheets.xlsx");

            workbook = new Workbook(Constants.sourcePath + "brateevo.json", options);

            Cells cells = workbook.Worksheets[0].Cells;
            Assert.AreEqual(cells["D5"].StringValue, "10к1");
            Assert.AreEqual(cells["D28"].StringValue, "11к1");
            Assert.AreEqual(cells["E16"].StringValue, "4");
            workbook.Save(Constants.destPath + "NET49861_out.xlsx");

        }
```

### See Also

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


