---
title: "PivotTable.PreserveFormatting"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Eigenschaft. Gibt an, ob die Zellformatierung PivotTableFormat beibehalten wird, wenn die PivotTable aktualisiert oder neu berechnet wird"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/preserveformatting/
---
## PivotTable.PreserveFormatting property

Gibt an, ob die Zellformatierung ([`PivotTableFormat`](../../pivottableformat/)) beibehalten wird, wenn die PivotTable aktualisiert oder neu berechnet wird.

```csharp
[Obsolete("Use PivotTable.PreserveCellFormattingOnUpdate property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool PreserveFormatting { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Bitte verwenden Sie stattdessen die Eigenschaft PivotTable.PreserveCellFormattingOnUpdate. Diese Methode wird 12 Monate nach Juli 2026 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPreserveFormattingDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook workbook = new Workbook("source.xlsx");
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greifen Sie auf die erste Pivot-Tabelle zu.
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // Beibehaltung der Formatierung während der Aktualisierung aktivieren
            pivotTable.PreserveFormatting = true;
            
            // Einige Formatierungen auf den Datenbereich der PivotTable anwenden
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.ForegroundColor = System.Drawing.Color.LightBlue;
            style.Pattern = BackgroundType.Solid;
            
            // Den Datenbereich der PivotTable formatieren
            pivotTable.FormatAll(style);
            
            // Pivot-Tabellendaten aktualisieren und berechnen
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


