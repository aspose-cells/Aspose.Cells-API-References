---
title: JsonLayoutOptions.ArrayAsTable
second_title: Aspose.Cells for .NET API Reference
description: JsonLayoutOptions property. Processes Array as table
type: docs
url: /net/aspose.cells.utility/jsonlayoutoptions/arrayastable/
---
## JsonLayoutOptions.ArrayAsTable property

Processes Array as table.

```csharp
public bool ArrayAsTable { get; set; }
```

### Examples

```csharp
// Called: JsonLayoutOptions options = new JsonLayoutOptions { ArrayAsTable = true };
[Test]
        public void Property_ArrayAsTable()
        {
            Workbook workbook = new Workbook();
            StreamReader streamReader = new StreamReader(File.OpenRead(Constants.sourcePath + "brateevo.json"));
            string sourcesJson = streamReader.ReadToEnd();
            JObject jObject = JObject.Parse(sourcesJson);
            foreach (var keyValuePair in jObject)
            {
                string json = keyValuePair.Value.ToString();

                Worksheet worksheet = workbook.Worksheets.Add(keyValuePair.Key);
                JsonLayoutOptions options = new JsonLayoutOptions { ArrayAsTable = true };
                JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
            }

            Assert.AreEqual(workbook.Worksheets[1].Cells["A1"].StringValue, "Братеево");
            Assert.AreEqual(workbook.Worksheets[2].Cells["A1"].StringValue, "com.westroom.entrycode.brateevo");

            Cells cells = workbook.Worksheets[3].Cells;
            Assert.AreEqual(cells["B4"].StringValue, "10к1");
            Assert.AreEqual(cells["B27"].StringValue, "11к1");
            Assert.AreEqual(cells["C15"].StringValue, "4");

            workbook.Save(Constants.destPath + "NET49865.xlsx");
        }
```

### See Also

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


