---
title: "JsonLayoutOptions.ConvertNumericOrDate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad JsonLayoutOptions. Indica si se convierte la cadena en json a valor numérico o de fecha"
type: docs
url: /es/net/aspose.cells.utility/jsonlayoutoptions/convertnumericordate/
---
## JsonLayoutOptions.ConvertNumericOrDate property

Indica si se convierte la cadena en json a un valor numérico o de fecha.

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### Ejemplos

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

### Ver también

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


