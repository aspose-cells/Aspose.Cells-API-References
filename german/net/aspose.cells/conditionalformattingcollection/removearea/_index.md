---
title: "ConditionalFormattingCollection.RemoveArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConditionalFormattingCollection-Methode. Entfernt alle bedingten Formatierungen im Bereich."
type: docs
url: /de/net/aspose.cells/conditionalformattingcollection/removearea/
---
## ConditionalFormattingCollection.RemoveArea method

Entfernt alle bedingten Formatierungen im Bereich.

```csharp
public void RemoveArea(int startRow, int startColumn, int totalRows, int totalColumns)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| startRow | Int32 | Die Startzeile des Bereichs. |
| startColumn | Int32 | Die Startspalte des Bereichs. |
| totalRows | Int32 | Die Anzahl der Zeilen des Bereichs. |
| totalColumns | Int32 | Die Anzahl der Spalten des Bereichs. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingCollectionMethodRemoveAreaWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erhalte die Sammlung der bedingten Formatierung
            ConditionalFormattingCollection cfc = worksheet.ConditionalFormattings;

            // Füge einige Regeln für bedingte Formatierung hinzu
            int index = cfc.Add();
            FormatConditionCollection fcc = cfc[index];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 5;
            area.EndColumn = 5;
            fcc.AddArea(area);

            try
            {
                // Rufe RemoveArea mit den Parametern (Int32, Int32, Int32, Int32) auf
                cfc.RemoveArea(0, 0, 3, 3);

                Console.WriteLine("Conditional formatting removed from area (0,0,3,3)");
                
                // Überprüfe die Wirkung, indem du die Anzahl prüfst (dies wäre 0, wenn alle Formatierungen entfernt wurden)
                Console.WriteLine($"Remaining conditional formatting areas: {fcc.RangeCount}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("RemoveAreaWithInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


