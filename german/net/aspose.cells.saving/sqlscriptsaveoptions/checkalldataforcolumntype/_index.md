---
title: "SqlScriptSaveOptions.CheckAllDataForColumnType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SqlScriptSaveOptions-Eigenschaft. Prüft alle Daten, um den Datentyp der Spalten zu ermitteln"
type: docs
url: /de/net/aspose.cells.saving/sqlscriptsaveoptions/checkalldataforcolumntype/
---
## SqlScriptSaveOptions.CheckAllDataForColumnType property

Überprüfe alle Daten, um den Datentyp der Spalten zu ermitteln.

```csharp
public bool CheckAllDataForColumnType { get; set; }
```

### Hinweise

Der Standardwert ist false, wir prüfen nur die erste Zeile aus Leistungsgründen. Wenn diese Eigenschaft true ist und die Spalten gemischte Werttypen enthalten, wird der Spaltentyp zu Text.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyCheckAllDataForColumnTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispielarbeitsmappe mit Testdaten
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Beispieldaten mit gemischten Typen hinzufügen
            sheet.Cells["A1"].PutValue("First_name");
            sheet.Cells["B1"].PutValue("Last_name");
            sheet.Cells["C1"].PutValue("age");
            sheet.Cells["D1"].PutValue("tax");
            
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["B2"].PutValue("Doe");
            sheet.Cells["C2"].PutValue(30);
            sheet.Cells["D2"].PutValue("10%");
            
            sheet.Cells["A3"].PutValue("Jane");
            sheet.Cells["B3"].PutValue("Smith");
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["D3"].PutValue(0.15);

            // SQL-Speicheroptionen konfigurieren
            SqlScriptSaveOptions sqlSaveOptions = new SqlScriptSaveOptions();
            sqlSaveOptions.OperatorType = SqlScriptOperatorType.Insert;
            sqlSaveOptions.CreateTable = true;
            sqlSaveOptions.CheckAllDataForColumnType = true; // This will examine all data to determine column types
            
            // Als SQL‑Skript speichern – Die Save‑Methode gibt keinen String zurück, daher müssen wir zuerst speichern und dann die Datei lesen
            wb.Save("output.sql", sqlSaveOptions);
            
            // Das erzeugte SQL‑Skript lesen
            string sqlScript = System.IO.File.ReadAllText("output.sql");
            
            Console.WriteLine("SQL Script generated:");
            Console.WriteLine(sqlScript);
        }
    }
}
```

### Siehe auch

* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


