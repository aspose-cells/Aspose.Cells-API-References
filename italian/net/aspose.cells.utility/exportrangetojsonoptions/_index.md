---
title: "Classe ExportRangeToJsonOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Utility.ExportRangeToJsonOptions. Indica le opzioni per l'esportazione dell'intervallo in JSON"
type: docs
url: /it/net/aspose.cells.utility/exportrangetojsonoptions/
---
## ExportRangeToJsonOptions class

Indica le opzioni per l'esportazione dell'intervallo in JSON.

```csharp
public class ExportRangeToJsonOptions
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ExportRangeToJsonOptions](exportrangetojsonoptions/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [ExportAsString](../../aspose.cells.utility/exportrangetojsonoptions/exportasstring/) { get; set; } | Esporta il valore stringa delle celle in JSON. |
| [ExportEmptyCells](../../aspose.cells.utility/exportrangetojsonoptions/exportemptycells/) { get; set; } | Indica se esportare le celle vuote come null. |
| [HasHeaderRow](../../aspose.cells.utility/exportrangetojsonoptions/hasheaderrow/) { get; set; } | Indica se l'intervallo contiene la riga di intestazione. |
| [Indent](../../aspose.cells.utility/exportrangetojsonoptions/indent/) { get; set; } | Indica l'indentazione. |

### Esempi

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Utility;

namespace AsposeCellsExamples
{
    public class UtilityClassExportRangeToJsonOptionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio alle celle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea opzioni di esportazione
            var exportOptions = new ExportRangeToJsonOptions();
            
            // Esporta intervallo in JSON
            var range = worksheet.Cells.CreateRange(0, 0, 3, 2);
            string jsonData = JsonUtility.ExportRangeToJson(range, exportOptions);

            // Genera il JSON
            Console.WriteLine("Exported JSON:");
            Console.WriteLine(jsonData);
            
            // Salva su file (opzionale)
            File.WriteAllText("exported_data.json", jsonData);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Utility](../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../)


