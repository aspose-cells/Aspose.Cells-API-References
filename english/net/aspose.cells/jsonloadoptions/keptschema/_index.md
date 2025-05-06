---
title: JsonLoadOptions.KeptSchema
second_title: Aspose.Cells for .NET API Reference
description: JsonLoadOptions property. Indicates whether keeping schema of this json
type: docs
url: /net/aspose.cells/jsonloadoptions/keptschema/
---
## JsonLoadOptions.KeptSchema property

Indicates whether keeping schema of this json.

```csharp
public bool KeptSchema { get; set; }
```

### Remarks

Sometimes we will save the file to JSON after loading JSON file.

### Examples

```csharp
// Called: loadOptions.KeptSchema = true;
[Test]
        public void Property_KeptSchema()
        {
            JsonLoadOptions loadOptions = new JsonLoadOptions();
            loadOptions.KeptSchema = true;

            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET56240.json&quot;, loadOptions);

            workbook.Save(Constants.destPath + &quot;CellsNet56241.xlsx&quot;);
              workbook = new Workbook(Constants.destPath + &quot;CellsNet56241.xlsx&quot;);
            workbook.Save(Constants.destPath + &quot;CELLSNET56240.json&quot;, new JsonSaveOptions()
            {

                ExportNestedStructure = true,
                SkipEmptyRows = true,
                  Schemas = new string[] { File.ReadAllText(Constants.sourcePath + &quot;CELLSNET56240.json&quot;) }
                //  AlwaysExportAsJsonObject = true
            });
            Assert.IsTrue(File.ReadAllText(Constants.destPath + &quot;CELLSNET56240.json&quot;).IndexOf(&quot; \&quot;CurrencyConfigurations1\&quot;:[{&quot;) != -1);

        }
```

### See Also

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


