---
title: "ConditionalFormattingValue.IsGTE"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConditionalFormattingValue‑Eigenschaft. Gibt das Größer‑oder‑Gleich‑Flag zurück oder legt es fest. Nur für Symbolsets verwenden; bestimmt, ob dieser Schwellenwert den Größer‑oder‑Gleich‑Operator verwendet. false bedeutet, dass stattdessen der Größer‑als‑Operator verwendet wird. Der Standardwert ist true."
type: docs
url: /de/net/aspose.cells/conditionalformattingvalue/isgte/
---
## ConditionalFormattingValue.IsGTE property

Abrufen oder Festlegen des Greater Than Or Equal‑Flags. Nur für Icon‑Sets verwenden, bestimmt, ob dieser Schwellenwert den Operator größer‑gleich verwendet. 'false' bedeutet, dass 'größer als' anstelle von 'größer‑gleich' verwendet wird. Der Standardwert ist true.

```csharp
public bool IsGTE { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyIsGTEDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet ws = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            ws.Cells["A1"].PutValue(1);
            ws.Cells["A2"].PutValue(2);
            ws.Cells["A3"].PutValue(3);
            ws.Cells["A4"].PutValue(4);
            ws.Cells["A5"].PutValue(5);

            // Bedingte Formatierung hinzufügen
            int index = ws.ConditionalFormattings.Add();
            FormatConditionCollection fcc = ws.ConditionalFormattings[index];
            fcc.AddArea(CellArea.CreateCellArea("A1", "A5"));

            // Erstelle ein Farbskalenformat
            index = fcc.AddCondition(FormatConditionType.ColorScale);
            FormatCondition fc = fcc[index];
            
            // Konfiguriere eine 2‑Farben‑Skala
            fc.ColorScale.Is3ColorScale = false;
            
            // Setze das Maximalwertformat (Demonstration von IsGTE)
            fc.ColorScale.MaxCfvo.IsGTE = true;
            fc.ColorScale.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.ColorScale.MaxColor = Color.Yellow;
            
            // Setze das Minimalwertformat
            fc.ColorScale.MinCfvo.IsGTE = true;
            fc.ColorScale.MinCfvo.Type = FormatConditionValueType.Min;
            fc.ColorScale.MinColor = Color.Red;

            // Speichere die Arbeitsmappe
            workbook.Save("ConditionalFormattingValuePropertyIsGTEDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


