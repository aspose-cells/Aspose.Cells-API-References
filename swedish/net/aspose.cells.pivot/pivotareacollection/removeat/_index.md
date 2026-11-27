---
title: "PivotAreaCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotAreaCollection-metod. Ta bort en pivotvillkorligt formaterad områdeinställning"
type: docs
url: /sv/net/aspose.cells.pivot/pivotareacollection/removeat/
---
## PivotAreaCollection.RemoveAt method

Ta bort en pivotvillkorligt formaterad områdeinställning.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Indexet |

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Lägg till en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // Definiera cellområden att lägga till i pivotområden.
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

            // Hämta samlingen av pivotområden genom att välja området.
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(cellArea1);
            pivotAreas.Add(cellArea2);

            try
            {
                // Visa pivotområden innan borttagning.
                Console.WriteLine("Pivot areas before removal:");
                for (int i = 0; i < pivotAreas.Count; i++)
                {
                    CellArea[] areas = pivotAreas[i].GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Area {i}: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }

                // Anropa RemoveAt-metoden med Int32-parameter
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

            // Spara resultatet
            workbook.Save("PivotAreaCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


