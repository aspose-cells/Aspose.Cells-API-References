---
title: JsonLayoutOptions.KeptSchema
second_title: Aspose.Cells for .NET API Reference
description: JsonLayoutOptions property. Indicates whether keeping schema of this json
type: docs
url: /net/aspose.cells.utility/jsonlayoutoptions/keptschema/
---
## JsonLayoutOptions.KeptSchema property

Indicates whether keeping schema of this json.

```csharp
public bool KeptSchema { get; set; }
```

### Remarks

Sometimes we will save the file to JSON after loading JSON file.

### Examples

```csharp
// Called: layoutOptions.KeptSchema = true;
[Test]
        public void Property_KeptSchema()
        {
            var workbook = new Workbook();
            workbook.Worksheets.Clear();
            var worksheet = workbook.Worksheets.Add(&quot;1&quot;);

            var data1 = new Data()
            {
                RootProperty = &quot;RootPropertyValue&quot;,
                Payload = new Payload()
                {
                    Array = new[]
                    {
                new ArrayData () { ArrayProperty = &quot;a1&quot; },
                new ArrayData () { ArrayProperty = &quot;a2&quot; },
                new ArrayData () { ArrayProperty = &quot;a3&quot; },
            },
                    PayloadProperty = &quot;PayloadPropertyValue&quot;,
                    PayloadStruct = new PayloadStruct()
                    {
                        PayloadProperty1 = &quot;val1&quot;,
                        PayloadProperty2 = &quot;val2&quot;
                    }
                }
            };

            var serializeObject = JsonConvert.SerializeObject(new[] { data1 });
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.KeptSchema = true;
            JsonUtility.ImportData(serializeObject, worksheet.Cells, 0, 0, layoutOptions);


            workbook.Save(Constants.destPath + &quot;CellsNet56124.xlsx&quot;, SaveFormat.Xlsx);
            workbook.Save(Constants.destPath + &quot;CellsNet56124.json&quot;, new JsonSaveOptions()
            {
                ExportNestedStructure = true,
                SkipEmptyRows = true,
                //   AlwaysExportAsJsonObject = true,
                ValidateMergedAreas = true,
            });
            string text = File.ReadAllText(Constants.destPath + &quot;CellsNet56124.json&quot;);
            Assert.IsTrue(text.IndexOf(&quot;\&quot;ArrayProperty\&quot;:\&quot;a1\&quot;&quot;) != -1);
        }
```

### See Also

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


