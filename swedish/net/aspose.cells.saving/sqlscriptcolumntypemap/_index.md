---
title: "Klass SqlScriptColumnTypeMap"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Saving.SqlScriptColumnTypeMap‑klass. Representerar kolumntypkarta"
type: docs
url: /sv/net/aspose.cells.saving/sqlscriptcolumntypemap/
---
## SqlScriptColumnTypeMap class

Representerar kolumntypkarta.

```csharp
public class SqlScriptColumnTypeMap
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [SqlScriptColumnTypeMap](sqlscriptcolumntypemap/)() | Standardkonstruktorn. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| virtual [GetNumbericType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/)() | (**Obsolete.**) Hämtar numerisk typ i databasen. |
| virtual [GetNumberType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumbertype/)() | Hämtar numerisk typ i databasen. |
| virtual [GetStringType](../../aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/)() | Hämtar strängtyp i databasen. |

### Exempel

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
            // Skapa en instans av SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Demonstrera användningen av GetStringType‑ och GetNumbericType‑metoderna
            string stringType = columnTypeMap.GetStringType();
            string numericType = columnTypeMap.GetNumbericType();

            // Skriv ut resultaten till konsolen
            Console.WriteLine("String Type in Database: " + stringType);
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // Skapa en instans av SqlScriptSaveOptions och ange ColumnTypeMap
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };

            // Skapa en arbetsbok och lägg till lite data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // Spara arbetsboken som SQL‑script med hjälp av sparalternativen
            workbook.Save("SqlScriptExample.sql", saveOptions);

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


