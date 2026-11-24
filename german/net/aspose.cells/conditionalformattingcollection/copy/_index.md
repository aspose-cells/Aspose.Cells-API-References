---
title: "ConditionalFormattingCollection.Copy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConditionalFormattingCollection-Methode. Kopiert die bedingte Formatierung"
type: docs
url: /de/net/aspose.cells/conditionalformattingcollection/copy/
---
## ConditionalFormattingCollection.Copy method

Kopiert die bedingte Formatierung.

```csharp
public void Copy(ConditionalFormattingCollection cfs)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cfs | ConditionalFormattingCollection | Die bedingte Formatierung |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingCollectionMethodCopyWithConditionalFormattingCollectioDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Erstelle eine Quellarbeitsmappe mit bedingter Formatierung
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];

            // Füge Beispiel für bedingte Formatierung zum Quellblatt hinzu
            int index = sourceSheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sourceSheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Erstelle und wende Stil auf die Formatbedingung an
            Style style = sourceWorkbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Red;
            FormatCondition fc = fcc[0];
            fc.Style = style;

            // Auf einen Bereich anwenden
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 5;
            area.StartColumn = 0;
            area.EndColumn = 5;
            fcc.AddArea(area);

            // Kopiere bedingte Formatierung von Quelle zu Ziel
            destSheet.ConditionalFormattings.Copy(sourceSheet.ConditionalFormattings);

            // Speichere die Arbeitsmappe
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


