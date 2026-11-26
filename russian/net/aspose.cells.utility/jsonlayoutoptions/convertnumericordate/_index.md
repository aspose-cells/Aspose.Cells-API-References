---
title: "JsonLayoutOptions.ConvertNumericOrDate"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство JsonLayoutOptions. Указывает, преобразовывать ли строку в JSON в числовое или датовое значение"
type: docs
url: /ru/net/aspose.cells.utility/jsonlayoutoptions/convertnumericordate/
---
## JsonLayoutOptions.ConvertNumericOrDate property

Указывает, следует ли преобразовать строку в json в числовое или датовое значение.

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class JsonLayoutOptionsPropertyConvertNumericOrDateDemo
    {
        public static void Run()
        {
            string jsonData = "[{\"ID\":101,\"Name\":\"John Doe\",\"BirthDate\":\"15-05-1990\",\"Salary\":75000.50}]";

            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            JsonLayoutOptions layoutOptions = new JsonLayoutOptions();
            layoutOptions.ArrayAsTable = true;
            layoutOptions.ConvertNumericOrDate = true;
            layoutOptions.DateFormat = "dd-MM-yyyy";
            layoutOptions.NumberFormat = "#,##0.00";

            JsonUtility.ImportData(jsonData, worksheet.Cells, 0, 0, layoutOptions);

            Console.WriteLine("Cell A2 (ID) type: " + worksheet.Cells["A2"].Type); // Should be numeric
            Console.WriteLine("Cell C2 (BirthDate) type: " + worksheet.Cells["C2"].Type); // Should be DateTime
            Console.WriteLine("Cell D2 (Salary) value: " + worksheet.Cells["D2"].Value); // Should be formatted number

            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


