---
title: "Enum SqlScriptOperatorType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Saving.SqlScriptOperatorType enum. Rappresenta il tipo di dati operativi"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptoperatortype/
---
## SqlScriptOperatorType enumeration

Rappresenta il tipo di dati operativi.

```csharp
public enum SqlScriptOperatorType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Insert | `0` | Inserisci dati. |
| Update | `1` | Aggiorna dati. |
| Delete | `2` | Elimina dati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptOperatorTypeDemo
    {
        public static void SqlScriptOperatorTypeExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Aggiungi un nuovo foglio di lavoro alla cartella di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // Crea SqlScriptSaveOptions e imposta le proprietà.
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                CheckIfTableExists = true,
                AddBlankLineBetweenRows = true,
                Separator = ';',
                OperatorType = SqlScriptOperatorType.Insert,
                PrimaryKey = 0,
                CreateTable = true,
                IdName = "ID",
                StartId = 1,
                TableName = "SampleTable",
                ExportAsString = false,
                ExportArea = new CellArea { StartRow = 1, StartColumn = 0, EndRow = 3, EndColumn = 1 },
                HasHeaderRow = true
            };

            // Salva la cartella di lavoro come script SQL.
            workbook.Save("SqlScriptOperatorTypeExample.sql", saveOptions);

            // Restituisci i risultati
            Console.WriteLine("SQL script has been saved successfully.");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


