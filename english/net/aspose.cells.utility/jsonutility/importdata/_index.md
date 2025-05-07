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
// Called: Aspose.Cells.Utility.JsonUtility.ImportData(inputJson, worksheet.Cells, row, column, options);
[Test]
        public void Method_JsonLayoutOptions_()
        {
            string inputJson = @"[
                                    { BEFORE: 'before cell', TEST: 'asd1', AFTER: 'after cell' },
                                    { BEFORE: 'before cell', TEST: 'asd2', AFTER: 'after cell' },
                                    { BEFORE: 'before cell', TEST: 'asd3', AFTER: 'after cell' },
                                    { BEFORE: 'before cell', TEST: 'asd4', AFTER: 'after cell' }
                                ]";
            string sheetName = "Sheet1";
            //int row = 0; // NO EXCEPTION
            int row = 1; //EXCEPTION if greater than 0
            int column = 0;

            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[sheetName];// ?? workbook.Worksheets.Add(sheetName);

            Aspose.Cells.Utility.JsonLayoutOptions options = new Aspose.Cells.Utility.JsonLayoutOptions { ArrayAsTable = true };
            Aspose.Cells.Utility.JsonUtility.ImportData(inputJson, worksheet.Cells, row, column, options);

            Assert.AreEqual(worksheet.Cells["A2"].StringValue, "BEFORE");
        }
```

### See Also

* class [Cells](../../../aspose.cells/cells/)
* class [JsonLayoutOptions](../../jsonlayoutoptions/)
* class [JsonUtility](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


