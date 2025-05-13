---
title: JsonLayoutOptions.DateFormat
second_title: Aspose.Cells for .NET API Reference
description: JsonLayoutOptions property. Gets and sets the format of date value
type: docs
url: /net/aspose.cells.utility/jsonlayoutoptions/dateformat/
---
## JsonLayoutOptions.DateFormat property

Gets and sets the format of date value.

```csharp
public string DateFormat { get; set; }
```

### Examples

```csharp
// Called: layoutOptions.DateFormat = ("DD-MM-YYYY");
public void JsonLayoutOptions_Property_DateFormat()
{
    Workbook workbook = new Workbook(FileFormatType.Xlsx);
    Worksheet worksheet = workbook.Worksheets[0];
    JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
    layoutOptions.ArrayAsTable = (true);
    layoutOptions.ConvertNumericOrDate = (true);
    layoutOptions.DateFormat = ("DD-MM-YYYY");
    JsonUtility.ImportData("{\"mongo_id\": \"5af05801b87fd\",\"date\" : \"01-09-2022\",\"AccountNumber\" : \"00000940104495187\"}", worksheet.Cells, 0, 0, layoutOptions);
    Cell cell = worksheet.Cells["C2"];
    Assert.AreEqual("00000940104495187", cell.StringValue);
    Assert.AreEqual(CellValueType.IsString, cell.Type);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


