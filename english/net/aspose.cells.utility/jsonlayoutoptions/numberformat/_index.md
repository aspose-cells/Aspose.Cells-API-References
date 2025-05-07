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
// Called: layoutOptions.NumberFormat = ("0");
[Test]
        public void Property_NumberFormat()
        {
            String data = "[{\"Employee Id\": \"T510\",\"First Name\": \"Darwinboxcore76\",\"Last Name\": \"Employee76\",\"Gender\": \"Male\"," +
                   "\"Date Of Birth\": \"24-02-1976\",\"Date Of Joining\": \"03-10-2022\",\"Date Of Exit\": \" \",\"Bank Account Number\": \"00000940104495187\",\"Bank Ifsc Code\": \" \"}]";

            Workbook workbook = new Workbook();
            workbook.Settings.Region = CountryCode.UnitedKingdom;
            Worksheet worksheet = workbook.Worksheets[0];
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.ArrayAsTable = (true);
            layoutOptions.ConvertNumericOrDate = (true);
            layoutOptions.NumberFormat = ("0");
            layoutOptions.DateFormat = ("DD-MMM-YYYY");
            JsonUtility.ImportData(data, worksheet.Cells, 0, 0, layoutOptions);

            Assert.AreEqual(CellValueType.IsDateTime, worksheet.Cells["E2"].Type);
            Assert.AreEqual(CellValueType.IsDateTime, worksheet.Cells["F2"].Type);
            Assert.AreEqual(CellValueType.IsString, worksheet.Cells["H2"].Type);


            workbook.Save(Constants.destPath + "CELLSNODEJSJAVA47.xlsx");
        }
```

### See Also

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


