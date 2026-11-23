---
title: "JsonLayoutOptions.ConvertNumericOrDate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété JsonLayoutOptions. Indique s'il faut convertir la chaîne dans le json en valeur numérique ou date"
type: docs
url: /fr/net/aspose.cells.utility/jsonlayoutoptions/convertnumericordate/
---
## JsonLayoutOptions.ConvertNumericOrDate property

Indique si la conversion de la chaîne en json en valeur numérique ou date est effectuée.

```csharp
public bool ConvertNumericOrDate { get; set; }
```

### Exemples

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

### Voir aussi

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


