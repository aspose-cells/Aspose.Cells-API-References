---
title: JsonLayoutOptions.NumberFormat
second_title: Aspose.Cells for .NET API Reference
description: JsonLayoutOptions property. Gets and sets the format of numeric value
type: docs
url: /net/aspose.cells.utility/jsonlayoutoptions/numberformat/
---
## JsonLayoutOptions.NumberFormat property

Gets and sets the format of numeric value.

```csharp
public string NumberFormat { get; set; }
```

### Examples

```csharp
// Called: layoutOptions.NumberFormat = (&amp;quot;0&amp;quot;);
[Test]
        public void Property_NumberFormat()
        {
            String data = &quot;[{\&quot;Employee Id\&quot;: \&quot;T510\&quot;,\&quot;First Name\&quot;: \&quot;Darwinboxcore76\&quot;,\&quot;Last Name\&quot;: \&quot;Employee76\&quot;,\&quot;Gender\&quot;: \&quot;Male\&quot;,&quot; +
                   &quot;\&quot;Date Of Birth\&quot;: \&quot;24-02-1976\&quot;,\&quot;Date Of Joining\&quot;: \&quot;03-10-2022\&quot;,\&quot;Date Of Exit\&quot;: \&quot; \&quot;,\&quot;Bank Account Number\&quot;: \&quot;00000940104495187\&quot;,\&quot;Bank Ifsc Code\&quot;: \&quot; \&quot;}]&quot;;

            Workbook workbook = new Workbook();
            workbook.Settings.Region = CountryCode.UnitedKingdom;
            Worksheet worksheet = workbook.Worksheets[0];
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.ArrayAsTable = (true);
            layoutOptions.ConvertNumericOrDate = (true);
            layoutOptions.NumberFormat = (&quot;0&quot;);
            layoutOptions.DateFormat = (&quot;DD-MMM-YYYY&quot;);
            JsonUtility.ImportData(data, worksheet.Cells, 0, 0, layoutOptions);

            Assert.AreEqual(CellValueType.IsDateTime, worksheet.Cells[&quot;E2&quot;].Type);
            Assert.AreEqual(CellValueType.IsDateTime, worksheet.Cells[&quot;F2&quot;].Type);
            Assert.AreEqual(CellValueType.IsString, worksheet.Cells[&quot;H2&quot;].Type);


            workbook.Save(Constants.destPath + &quot;CELLSNODEJSJAVA47.xlsx&quot;);
        }
```

### See Also

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


