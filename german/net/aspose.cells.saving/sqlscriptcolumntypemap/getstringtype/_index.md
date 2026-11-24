---
title: "SqlScriptColumnTypeMap.GetStringType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SqlScriptColumnTypeMap‑Methode. Gibt den Zeichenkettentyp in der Datenbank zurück"
type: docs
url: /de/net/aspose.cells.saving/sqlscriptcolumntypemap/getstringtype/
---
## SqlScriptColumnTypeMap.GetStringType method

Gibt den Zeichenkettentyp in der Datenbank zurück.

```csharp
public virtual string GetStringType()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptColumnTypeMapMethodGetStringTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Abrufen und Anzeigen des Standard‑Zeichenkettentyps
            string stringType = columnTypeMap.GetStringType();
            Console.WriteLine("Default String Type: " + stringType);

            // Erstelle eine einfache Arbeitsmappe mit Zeichenkettendaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John Doe");

            // Speichern mit SQL‑Skript‑Optionen unter Verwendung der Typzuordnung
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            
            workbook.Save("SqlScriptOutput.sql", saveOptions);
            Console.WriteLine("SQL script saved with string type: " + stringType);
        }
    }
}
```

### Siehe auch

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


