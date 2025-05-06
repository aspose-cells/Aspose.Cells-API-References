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
// Called: JsonUtility.ImportData(File.ReadAllText(Constants.sourcePath + &amp;quot;CellsNet47462.txt&amp;quot;), workbook.Worksheets[0].Cells, 0, 0, options); //Error occurs here
[Test]
        public void Method_JsonLayoutOptions_()
        {
            //Create workbook
            Workbook workbook = new Workbook();
            //Worksheet worksheet = workbook.Worksheets[0];

            //Read JSON files
            JsonLayoutOptions options = new JsonLayoutOptions();

            //Import JSON data
            JsonUtility.ImportData(File.ReadAllText(Constants.sourcePath + &quot;CellsNet47462.txt&quot;), workbook.Worksheets[0].Cells, 0, 0, options); //Error occurs here

            workbook.Save(Constants.destPath + &quot;CellsNet47462.xlsx&quot;);

        }
```

### See Also

* class [Cells](../../../aspose.cells/cells/)
* class [JsonLayoutOptions](../../jsonlayoutoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


