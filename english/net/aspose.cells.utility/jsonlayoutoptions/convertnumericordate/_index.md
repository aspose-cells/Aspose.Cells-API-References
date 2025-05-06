---
title: JsonLayoutOptions.ConvertNumericOrDate
second_title: Aspose.Cells for .NET API Reference
description: JsonLayoutOptions property. Indicates whether converting the string in json to numeric or date value
type: docs
url: /net/aspose.cells.utility/jsonlayoutoptions/convertnumericordate/
---
## JsonLayoutOptions.ConvertNumericOrDate property

Indicates whether converting the string in json to numeric or date value.

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### Examples

```csharp
// Called: layoutOptions.ConvertNumericOrDate = (true);
[Test]
        public void Property_ConvertNumericOrDate()
        {
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = workbook.Worksheets[0];
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.ArrayAsTable = (true);
            layoutOptions.ConvertNumericOrDate = (true);
            layoutOptions.DateFormat = (&quot;DD-MM-YYYY&quot;);
            JsonUtility.ImportData(&quot;{\&quot;mongo_id\&quot;: \&quot;5af05801b87fd\&quot;,\&quot;date\&quot; : \&quot;01-09-2022\&quot;,\&quot;AccountNumber\&quot; : \&quot;00000940104495187\&quot;}&quot;, worksheet.Cells, 0, 0, layoutOptions);
            Cell cell = worksheet.Cells[&quot;C2&quot;];
            Assert.AreEqual(&quot;00000940104495187&quot;, cell.StringValue);
            Assert.AreEqual(CellValueType.IsString, cell.Type);
            workbook.Save(Constants.destPath + &quot;CELLSNET53268.xlsx&quot;);
        }
```

### See Also

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


