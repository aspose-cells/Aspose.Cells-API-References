---
title: "Klasse SqlScriptColumnTypeMap"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Saving.SqlScriptColumnTypeMap Klasse. Stellt die Spaltentypzuordnung dar"
type: docs
url: /de/net/aspose.cells.saving/sqlscriptcolumntypemap/
---
## SqlScriptColumnTypeMap class

Stellt die Spaltentypzuordnung dar.

```csharp
public class SqlScriptColumnTypeMap
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [SqlScriptColumnTypeMap](sqlscriptcolumntypemap/)() | Der Standardkonstruktor. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| virtual [GetNumbericType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/)() | (**Obsolete.**) Gibt den numerischen Typ in der Datenbank zurück. |
| virtual [GetNumberType](../../aspose.cells.saving/sqlscriptcolumntypemap/getnumbertype/)() | Gibt den numerischen Typ in der Datenbank zurück. |
| virtual [GetStringType](../../aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/)() | Gibt den Zeichenkettentyp in der Datenbank zurück. |

### Beispiele

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
            // Erstelle eine Instanz von SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Demonstriere die Verwendung der Methoden GetStringType und GetNumbericType
            string stringType = columnTypeMap.GetStringType();
            string numericType = columnTypeMap.GetNumbericType();

            // Gib die Ergebnisse in der Konsole aus
            Console.WriteLine("String Type in Database: " + stringType);
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // Erstelle eine Instanz von SqlScriptSaveOptions und setze die ColumnTypeMap
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };

            // Erstellen Sie eine Arbeitsmappe und fügen Sie einige Daten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Doe");

            // Speichere die Arbeitsmappe als SQL-Skript unter Verwendung der Speicheroptionen
            workbook.Save("SqlScriptExample.sql", saveOptions);

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Saving](../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../)


