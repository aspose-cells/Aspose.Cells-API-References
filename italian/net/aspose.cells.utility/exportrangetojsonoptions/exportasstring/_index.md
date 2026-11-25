---
title: "ExportRangeToJsonOptions.ExportAsString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ExportRangeToJsonOptions. Esporta il valore stringa delle celle in json"
type: docs
url: /it/net/aspose.cells.utility/exportrangetojsonoptions/exportasstring/
---
## ExportRangeToJsonOptions.ExportAsString property

Esporta il valore stringa delle celle in JSON.

```csharp
public bool ExportAsString { get; set; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class ExportRangeToJsonOptionsPropertyExportAsStringDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola le celle con diversi tipi di dati
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("String");
            worksheet.Cells["B2"].PutValue("Hello");
            worksheet.Cells["A3"].PutValue("Number");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["A4"].PutValue("Date");
            worksheet.Cells["B4"].PutValue(DateTime.Now);

            // Crea un'istanza di ExportRangeToJsonOptions
            ExportRangeToJsonOptions options = new ExportRangeToJsonOptions();
            options.HasHeaderRow = true;

            // Mostra il valore corrente di ExportAsString
            Console.WriteLine("Current ExportAsString value: " + options.ExportAsString);

            // Esporta senza ExportAsString (comportamento predefinito)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B4");
            string jsonWithoutString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON without ExportAsString:\n" + jsonWithoutString);

            // Imposta ExportAsString a true
            options.ExportAsString = true;

            // Esporta con ExportAsString
            string jsonWithString = JsonUtility.ExportRangeToJson(range, options);
            Console.WriteLine("JSON with ExportAsString:\n" + jsonWithString);

            // Salva la cartella di lavoro
            workbook.Save("ExportAsStringDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ExportRangeToJsonOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


