---
title: "SqlScriptSaveOptions.OperatorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SqlScriptSaveOptions-Eigenschaft. Liest und setzt den Operator-Typ von SQL"
type: docs
url: /de/net/aspose.cells.saving/sqlscriptsaveoptions/operatortype/
---
## SqlScriptSaveOptions.OperatorType property

Liest und setzt den Operator‑Typ des SQL.

```csharp
public SqlScriptOperatorType OperatorType { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Saving;

namespace AsposeCellsExamples
{
    public class SqlScriptSaveOptionsPropertyOperatorTypeDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispielarbeitsmappe mit Testdaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Id");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Jane");

            // SQL-Speicheroptionen konfigurieren
            SqlScriptSaveOptions options = new SqlScriptSaveOptions();
            options.OperatorType = SqlScriptOperatorType.Delete;
            options.IdName = "Id";
            options.Separator = '\n';
            options.AddBlankLineBetweenRows = true;
            options.CreateTable = true;

            // In Memory-Stream speichern und das SQL-Skript als Zeichenkette erhalten
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, options);
                stream.Position = 0;
                using (StreamReader reader = new StreamReader(stream))
                {
                    string sqlScript = reader.ReadToEnd();
                    
                    // Geben Sie das erzeugte SQL aus
                    Console.WriteLine("Generated SQL Script:");
                    Console.WriteLine(sqlScript);
                }
            }
        }
    }
}
```

### Siehe auch

* enum [SqlScriptOperatorType](../../sqlscriptoperatortype/)
* class [SqlScriptSaveOptions](../)
* namespace [Aspose.Cells.Saving](../../../aspose.cells.saving/)
* assembly [Aspose.Cells](../../../)


