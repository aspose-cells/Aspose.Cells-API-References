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

            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET56240.json", loadOptions);

            workbook.Save(Constants.destPath + "CellsNet56241.xlsx");
              workbook = new Workbook(Constants.destPath + "CellsNet56241.xlsx");
            workbook.Save(Constants.destPath + "CELLSNET56240.json", new JsonSaveOptions()
            {

                ExportNestedStructure = true,
                SkipEmptyRows = true,
                  Schemas = new string[] { File.ReadAllText(Constants.sourcePath + "CELLSNET56240.json") }
                //  AlwaysExportAsJsonObject = true
            });
            Assert.IsTrue(File.ReadAllText(Constants.destPath + "CELLSNET56240.json").IndexOf(" \"CurrencyConfigurations1\":[{") != -1);

        }
```

### See Also

* class [JsonLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


