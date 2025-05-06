---
title: Class JsonLayoutOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Utility.JsonLayoutOptions class. Represents the options of json layout type
type: docs
url: /net/aspose.cells.utility/jsonlayoutoptions/
---
## JsonLayoutOptions class

Represents the options of json layout type.

```csharp
public class JsonLayoutOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [JsonLayoutOptions](jsonlayoutoptions/)() | Constructor of loading JSON layout options. |

## Properties

| Name | Description |
| --- | --- |
| [ArrayAsTable](../../aspose.cells.utility/jsonlayoutoptions/arrayastable/) { get; set; } | Processes Array as table. |
| [ConvertNumericOrDate](../../aspose.cells.utility/jsonlayoutoptions/convertnumericordate/) { get; set; } | Indicates whether converting the string in json to numeric or date value. |
| [DateFormat](../../aspose.cells.utility/jsonlayoutoptions/dateformat/) { get; set; } | Gets and sets the format of date value. |
| [IgnoreArrayTitle](../../aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/) { get; set; } | (**Obsolete.**) Indicates whether ignore title if array is a property of object. |
| [IgnoreNull](../../aspose.cells.utility/jsonlayoutoptions/ignorenull/) { get; set; } | Indicates whether ignoring null value. |
| [IgnoreObjectTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/) { get; set; } | (**Obsolete.**) Indicates whether ignore title if object is a property of object. |
| [IgnoreTitle](../../aspose.cells.utility/jsonlayoutoptions/ignoretitle/) { get; set; } | Ingores titles of attributes |
| [KeptSchema](../../aspose.cells.utility/jsonlayoutoptions/keptschema/) { get; set; } | Indicates whether keeping schema of this json. |
| [NumberFormat](../../aspose.cells.utility/jsonlayoutoptions/numberformat/) { get; set; } | Gets and sets the format of numeric value. |
| [TitleStyle](../../aspose.cells.utility/jsonlayoutoptions/titlestyle/) { get; set; } | Gets and sets the style of the title. |

### Examples

```csharp
// Called: JsonLayoutOptions options = new JsonLayoutOptions { ArrayAsTable = true };
[Test]
        public void Type_JsonLayoutOptions()
        {
            Workbook workbook = new Workbook();
            StreamReader streamReader = new StreamReader(File.OpenRead(Constants.sourcePath + &quot;brateevo.json&quot;));
            string sourcesJson = streamReader.ReadToEnd();
            JObject jObject = JObject.Parse(sourcesJson);
            foreach (var keyValuePair in jObject)
            {
                string json = keyValuePair.Value.ToString();

                Worksheet worksheet = workbook.Worksheets.Add(keyValuePair.Key);
                JsonLayoutOptions options = new JsonLayoutOptions { ArrayAsTable = true };
                JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
            }

            Assert.AreEqual(workbook.Worksheets[1].Cells[&quot;A1&quot;].StringValue, &quot;Братеево&quot;);
            Assert.AreEqual(workbook.Worksheets[2].Cells[&quot;A1&quot;].StringValue, &quot;com.westroom.entrycode.brateevo&quot;);

            Cells cells = workbook.Worksheets[3].Cells;
            Assert.AreEqual(cells[&quot;B4&quot;].StringValue, &quot;10к1&quot;);
            Assert.AreEqual(cells[&quot;B27&quot;].StringValue, &quot;11к1&quot;);
            Assert.AreEqual(cells[&quot;C15&quot;].StringValue, &quot;4&quot;);

            workbook.Save(Constants.destPath + &quot;NET49865.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


