---
title: "PivotTable.GetHorizontalBreaks"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotTable-Methode. Gibt die Zeilenindexliste der horizontalen Seitenumbrüche der Pivot-Tabelle zurück"
type: docs
url: /de/net/aspose.cells.pivot/pivottable/gethorizontalbreaks/
---
## PivotTable.GetHorizontalBreaks method

Gibt die Zeilenindexliste der horizontalen Seitenumbrüche der Pivot-Tabelle zurück

```csharp
[Obsolete("Use ivotTable.GetHorizontalPageBreaks() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList GetHorizontalBreaks()
```

### Hinweise

HINWEIS: Diese Methode ist jetzt veraltet. Verwenden Sie stattdessen die PivotTable.GetHorizontalPageBreaks()-Methode. Diese Methode wird 12 Monate später, seit Dezember 2024, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Collections;

    public class PivotTableMethodGetHorizontalBreaksDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die PivotTable hinzufügen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);
            worksheet.Cells["B5"].PutValue(4000);

            // Erstelle eine Pivot-Tabelle
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Füge Felder zur Pivot-Tabelle hinzu
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Daten berechnen, um die Pivot-Tabelle zu füllen
            pivotTable.CalculateData();

            try
            {
                // Hole horizontale Unterbrechungen (Seitenumbrüche) für die Pivot-Tabelle
                ArrayList horizontalBreaks = pivotTable.GetHorizontalBreaks();
                
                Console.WriteLine("Horizontal breaks (row indices):");
                foreach (int rowIndex in horizontalBreaks)
                {
                    Console.WriteLine(rowIndex);
                }

                // Füge zur Demonstration einen Seitenumbruch in Zeile 3 ein
                worksheet.HorizontalPageBreaks.Add("A3");
                
                // Hole aktualisierte horizontale Unterbrechungen
                horizontalBreaks = pivotTable.GetHorizontalBreaks();
                Console.WriteLine("\nHorizontal breaks after adding page break:");
                foreach (int rowIndex in horizontalBreaks)
                {
                    Console.WriteLine(rowIndex);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetHorizontalBreaks method: {ex.Message}");
            }
            
            // Ergebnis speichern
            workbook.Save("PivotTableGetHorizontalBreaksDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


