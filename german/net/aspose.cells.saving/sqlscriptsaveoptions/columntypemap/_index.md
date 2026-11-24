---
title: "SqlScriptSaveOptions.ColumnTypeMap"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SqlScriptSaveOptions-Eigenschaft. Liefert und setzt die Zuordnung von Spaltentypen für verschiedene Datenbanken"
type: docs
url: /de/net/aspose.cells.saving/sqlscriptsaveoptions/columntypemap/
---
## SqlScriptSaveOptions.ColumnTypeMap property

Liest und setzt die Zuordnung von Spaltentypen für verschiedene Datenbanken.

```csharp
public SqlScriptColumnTypeMap ColumnTypeMap { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyColumnTypeMapDemo
    {
        public static void Run()
        {
            // Erstelle eine benutzerdefinierte Spaltentypzuordnung
            SqlScriptColumnTypeMap customTypeMap = new SqlScriptColumnTypeMap();
            
            // SQL-Speicheroptionen erstellen
            SqlScriptSaveOptions saveOptions = new SqlScriptSaveOptions
            {
                TableName = "Employees",
                CreateTable = true,
                ColumnTypeMap = customTypeMap,
                CheckIfTableExists = true,
                ExportAsString = false
            };

            // Beispiel-Arbeitsmappe mit Daten erstellen
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kopfzeilen hinzufügen
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["C1"].PutValue("Salary");
            
            // Datenzeilen hinzufügen
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John Smith");
            worksheet.Cells["C2"].PutValue(5000.50);
            
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane Doe");
            worksheet.Cells["C3"].PutValue(6500.75);

            // Als SQL-Skript speichern
            workbook.Save("EmployeeData.sql", saveOptions);
            
            Console.WriteLine("SQL script generated successfully with custom column type mapping.");
        }
    }
}
```

### Siehe auch

* class [SqlScriptColumnTypeMap](../../sqlscriptcolumntypemap/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


