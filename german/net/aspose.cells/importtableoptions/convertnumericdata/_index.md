---
title: "ImportTableOptions.ConvertNumericData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImportTableOptions-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob der Zeichenfolgenwert in einen numerischen oder Datumswert konvertiert werden soll"
type: docs
url: /de/net/aspose.cells/importtableoptions/convertnumericdata/
---
## ImportTableOptions.ConvertNumericData property

Liest oder legt einen Wert fest, der angibt, ob der Zeichenfolgenwert in einen numerischen oder Datumswert konvertiert werden soll.

```csharp
public bool ConvertNumericData { get; set; }
```

### Beispiele

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ImportTableOptionsPropertyConvertNumericDataDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstelle eine Beispieltabelle mit numerischen und Zeichenfolgenwerten
            DataTable dt = new DataTable();
            dt.Columns.Add("Numbers");
            dt.Columns.Add("Text");
            dt.Rows.Add("123", "456");
            dt.Rows.Add("ABC", "DEF");

            // Holen Sie die Zellen des ersten Arbeitsblatts
            Cells cells = workbook.Worksheets[0].Cells;

            // Erstellen Sie Importoptionen mit ConvertNumericData auf true gesetzt
            ImportTableOptions options = new ImportTableOptions();
            options.ConvertNumericData = true;
            options.IsFieldNameShown = true;

            // Daten mit numerischer Konvertierung importieren
            cells.ImportData(dt, 0, 0, options);

            // Ergebnisse anzeigen
            Console.WriteLine("A2 (numeric converted): " + cells["A2"].Value + " - Type: " + cells["A2"].Type);
            Console.WriteLine("B2 (string remains): " + cells["B2"].StringValue + " - Type: " + cells["B2"].Type);
        }
    }
}
```

### Siehe auch

* class [ImportTableOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


