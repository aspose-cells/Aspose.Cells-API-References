---
title: "PivotAreaCollection.RemoveAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PivotAreaCollection-Methode. Entfernt eine Pivot‑bedingte formatierte Bereichseinstellung"
type: docs
url: /de/net/aspose.cells.pivot/pivotareacollection/removeat/
---
## PivotAreaCollection.RemoveAt method

Entfernt eine Pivot‑bedingte formatierte Bereichseinstellung.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Der Index |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für Pivot‑Tabelle erstellen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Fügen Sie eine Pivot-Tabelle hinzu
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Definieren Sie Zellbereiche, die zu Pivot‑Bereichen hinzugefügt werden
            CellArea cellArea1 = new CellArea();
            cellArea1.StartRow = 0;
            cellArea1.StartColumn = 0;
            cellArea1.EndRow = 2;
            cellArea1.EndColumn = 1;

            CellArea cellArea2 = new CellArea();
            cellArea2.StartRow = 1;
            cellArea2.StartColumn = 1;
            cellArea2.EndRow = 3;
            cellArea2.EndColumn = 2;

            // Abrufen der Pivot‑Bereich‑Sammlung durch Auswahl des Bereichs
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(cellArea1);
            pivotAreas.Add(cellArea2);

            try
            {
                // Anzeige der Pivot‑Bereiche vor dem Entfernen
                Console.WriteLine("Pivot areas before removal:");
                for (int i = 0; i < pivotAreas.Count; i++)
                {
                    CellArea[] areas = pivotAreas[i].GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Area {i}: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }

                // Rufen Sie die RemoveAt-Methode mit dem Int32-Parameter auf
                pivotAreas.RemoveAt(0);

                Console.WriteLine("\nPivot areas after removal:");
                for (int i = 0; i < pivotAreas.Count; i++)
                {
                    CellArea[] areas = pivotAreas[i].GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Area {i}: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("PivotAreaCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


