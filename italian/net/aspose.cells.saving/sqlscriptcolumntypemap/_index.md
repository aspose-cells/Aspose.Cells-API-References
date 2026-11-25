---
title: "Classe SqlScriptColumnTypeMap"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Saving.SqlScriptColumnTypeMap. Rappresenta la mappatura dei tipi di colonna"
type: docs
url: /it/net/aspose.cells.saving/sqlscriptcolumntypemap/
---
## SqlScriptColumnTypeMap class

Rappresenta la mappa dei tipi di colonna.

```csharp
public class SqlScriptColumnTypeMap
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SqlScriptColumnTypeMap](sqlscriptcolumntypemap/)() | Il costruttore predefinito. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| virtual [GetNumbericType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/)() | (**Obsoleto.**) Ottiene il tipo numerico nel database. |
| virtual [GetNumberType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumbertype/)() | Ottiene il tipo numerico nel database. |
| virtual [GetStringType](../../aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/)() | Ottiene il tipo stringa nel database. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Saving;
    using System;

    public class SqlScriptColumnTypeMapDemo
    {
        public static void SqlScriptColumnTypeMapExample()
        {
            // Crea un'istanza di SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Dimostra l'uso dei metodi GetStringType e GetNumbericType
            string stringType = columnTypeMap.GetStringType();
            string numericType = columnTypeMap.GetNumbericType();

            // Stampa i risultati sulla console
            Console.WriteLine("String Type in Database: " + stringType);
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // Crea un'istanza di SqlScriptSaveOptions e imposta ColumnTypeMap
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };

            // Crea una cartella di lavoro e aggiungi alcuni dati
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // Salva la cartella di lavoro come script SQL utilizzando le opzioni di salvataggio
            workbook.Save("SqlScriptExample.sql", saveOptions);

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


