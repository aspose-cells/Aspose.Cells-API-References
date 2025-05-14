---
title: JsonUtility.ImportData
second_title: Aspose.Cells for .NET API Reference
description: JsonUtility method. Import the json string
type: docs
url: /net/aspose.cells.utility/jsonutility/importdata/
---
## JsonUtility.ImportData method

Import the json string.

```csharp
public static int[] ImportData(string json, Cells cells, int row, int column, 
    JsonLayoutOptions option)
```

| Parameter | Type | Description |
| --- | --- | --- |
| json | String | The json string. |
| cells | Cells | The Cells. |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
| option | JsonLayoutOptions | The options of import json string. |

### Examples

```csharp
// Called: JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);
public void JsonUtility_Method_ImportData()
{
    string jsonInput = "[{"
                        + "\"Name\" : \"Name\","
                        + "\"DisplayName\" : \"DisplayName\","
                        + "\"ShowDisplayName\" : false"
                        + "},"
                        + "{"
                        + "\"Name\" : \"Nameone\","
                        + "\"DisplayName\" : \"DisplayNameone\","
                        + "\"ShowDisplayName\" : true"
                        + "},"
                        + "{"
                        + "\"Name\" : \"Nametwo\","
                        + "\"DisplayName\" : \"DisplayNametwo\","
                        + "\"ShowDisplayName\" : false"
                        + "}]";
    Workbook workbook = new Workbook();
    Worksheet worksheet = workbook.Worksheets[0];
    JsonLayoutOptions options = new JsonLayoutOptions();
    options.ArrayAsTable = true;
    JsonUtility.ImportData(jsonInput, worksheet.Cells, 0, 0, options);
    workbook.Save(Constants.destPath + "example.xlsx");

    Cells cells = workbook.Worksheets[0].Cells;
    Assert.AreEqual(cells["C3"].StringValue, "TRUE");
    Assert.AreEqual(cells["C4"].StringValue, "FALSE");
}
```

### See Also

* class [Cells](../../../aspose.cells/cells/)
* class [JsonLayoutOptions](../../jsonlayoutoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


