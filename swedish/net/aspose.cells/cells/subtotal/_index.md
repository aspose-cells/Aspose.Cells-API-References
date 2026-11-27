---
title: "Cells.Subtotal"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cells-metod. Skapar delsummer för intervallet"
type: docs
url: /sv/net/aspose.cells/cells/subtotal/
---
## Subtotal(CellArea, int, ConsolidationFunction, int[]) {#subtotal}

Skapar delsummer för intervallet.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | CellArea | Området |
| groupBy | Int32 | Fältet att gruppera efter, som ett nollbaserat heltalsavstånd |
| funktion | ConsolidationFunction | Delssummafunktionen. |
| totalList | Int32[] | En array av nollbaserade fältavstånd, som anger vilka fält som delsummeringar läggs till. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i exempeldata för delsummering
            CreateSampleData(worksheet);

            // Definiera cellområde som innehåller data (A1:C6)
            CellArea cellArea = CellArea.CreateCellArea(0, 0, 5, 2);

            try
            {
                // Anropa Subtotal-metoden med parametrar:
                // - Gruppera efter kolumn 0 (Region)
                // - Använd SUM-funktionen
                // - Tillämpa på kolumn 2 (Försäljning)
                worksheet.Cells.Subtotal(
                    cellArea,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 }
                );

                Console.WriteLine("Subtotal added successfully for parameters (CellArea, 0, Sum, [2])");
                
                // Metoderna ExpandColumnLevel och ExpandRowLevel togs bort för att åtgärda kompileringsfel
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Subtotal method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo.xlsx");
        }

        private static void CreateSampleData(Worksheet worksheet)
        {
            // Skapa rubrikrad
            worksheet.Cells["A1"].PutValue("Region");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");

            // Skapa datarader
            object[,] data = new object[,] {
                {"North", "Widget", 5000},
                {"North", "Gadget", 3000},
                {"South", "Widget", 6000},
                {"South", "Gadget", 4000},
                {"West", "Widget", 4500}
            };

            // Fyll i data med start från rad 2 (nollbaserat index 1)
            for (int i = 0; i < data.GetLength(0); i++)
            {
                worksheet.Cells[i + 1, 0].PutValue(data[i, 0]);
                worksheet.Cells[i + 1, 1].PutValue(data[i, 1]);
                worksheet.Cells[i + 1, 2].PutValue(data[i, 2]);
            }
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Subtotal(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) {#subtotal_1}

Skapar delsummer för intervallet.

```csharp
public void Subtotal(CellArea ca, int groupBy, ConsolidationFunction function, int[] totalList, 
    bool replace, bool pageBreaks, bool summaryBelowData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| ca | CellArea | Området |
| groupBy | Int32 | Fältet att gruppera efter, som ett nollbaserat heltalsavstånd |
| funktion | ConsolidationFunction | Delssummafunktionen. |
| totalList | Int32[] | En array av nollbaserade fältavstånd, som anger vilka fält som delsummeringar läggs till. |
| replace | Boolean | Anger om de nuvarande delsummerna ska ersättas |
| pageBreaks | Boolean | Anger om en sidbrytning ska läggas till mellan grupper |
| summaryBelowData | Boolean | Anger om en sammanfattning ska läggas till under data. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodSubtotalWithCellAreaInt32ConsolidationFuncDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Skapa exempeldata för delsummering
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Product");
            cells["C1"].PutValue("Sales");
            
            object[,] data = new object[,] {
                { "Fruits", "Apple", 1500 },
                { "Fruits", "Orange", 2500 },
                { "Vegetables", "Carrot", 1800 },
                { "Vegetables", "Potato", 3000 },
                { "Fruits", "Banana", 2000 }
            };

            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 3; col++)
                {
                    cells[row + 1, col].PutValue(data[row, col]);
                }
            }

            try
            {
                // Definiera cellområde för delsummering (A1:C6)
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 5;
                area.EndColumn = 2;

                // Anropa Subtotal med parametrar:
                // - Gruppera efter första kolumnen (0-baserat index 0)
                // - Använd Sum-funktionen
                // - Tillämpa på tredje kolumnen (0-baserat index 2)
                // - Ersätt befintliga delsummer, sidbrytningar mellan grupper, sammanfattning under data
                cells.Subtotal(
                    area,
                    0,
                    ConsolidationFunction.Sum,
                    new int[] { 2 },
                    true,
                    true,
                    true
                );

                Console.WriteLine("Subtotal added successfully for parameters: (CellArea, Int32, ConsolidationFunction, Int32[], Boolean, Boolean, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating subtotal: {ex.Message}");
            }

            workbook.Save("SubtotalDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* enum [ConsolidationFunction](../../consolidationfunction/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


