---
title: "PivotField.Position"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotField-Eigenschaft. Gibt den Index des PivotField im Bereich an"
type: docs
url: /de/net/aspose.cells.pivot/pivotfield/position/
---
## PivotField.Position property

Gibt den Index von [`PivotField`](../) im Bereich an.

```csharp
public int Position { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyPositionDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe aus einer Quell‑Excel‑Datei
            Workbook wb = new Workbook("NET46429_a.xlsx");
            
            // Zugriff auf das erste Arbeitsblatt und seine Pivot-Tabelle
            Worksheet ws = wb.Worksheets[0];
            PivotTable pt = ws.PivotTables[0];
            
            // Demonstriere die Verwendung der Position-Eigenschaft
            int position = pt.PageFields[0].Position;
            Console.WriteLine("Position of first page field: " + position);
            
            // Verwende Position, um Berichtfilterseiten anzuzeigen
            pt.ShowReportFilterPageByIndex(position);
            
            // Speichere die Arbeitsmappe
            wb.Save("PivotFieldPropertyPositionDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


