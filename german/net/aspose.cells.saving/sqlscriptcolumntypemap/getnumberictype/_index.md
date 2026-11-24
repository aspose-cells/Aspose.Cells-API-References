---
title: "SqlScriptColumnTypeMap.GetNumbericType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SqlScriptColumnTypeMap‑Methode. Gibt den numerischen Typ in der Datenbank zurück"
type: docs
url: /de/net/aspose.cells.saving/sqlscriptcolumntypemap/getnumberictype/
---
## SqlScriptColumnTypeMap.GetNumbericType method

Gibt den numerischen Typ in der Datenbank zurück.

```csharp
[Obsolete("Use SqlScriptColumnTypeMap.GetNumberType() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual string GetNumbericType()
```

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Bitte verwenden Sie stattdessen die Methode SqlScriptColumnTypeMap.GetNumberType(). Diese Methode wird 6 Monate später, seit Juli 2026, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptColumnTypeMapMethodGetNumbericTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von SqlScriptColumnTypeMap
            SqlScriptColumnTypeMap columnTypeMap = new SqlScriptColumnTypeMap();

            // Abrufen und Anzeigen der numerischen Typzuordnung
            string numericType = columnTypeMap.GetNumbericType();
            Console.WriteLine("Numeric Type in Database: " + numericType);

            // Erstelle eine einfache Arbeitsmappe mit numerischen Daten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Number");
            worksheet.Cells["A2"].PutValue(123.45);

            // Speichern mit SQL‑Skript‑Optionen unter Verwendung der Typzuordnung
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                ColumnTypeMap = columnTypeMap
            };
            workbook.Save("NumericTypeDemo.sql", saveOptions);
        }
    }
}
```

### Siehe auch

* class [SqlScriptColumnTypeMap](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


