---
title: "Cell.Equals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑metod. Kontrollerar om detta objekt refererar till samma cell som ett annat"
type: docs
url: /sv/net/aspose.cells/cell/equals/
---
## Equals(object) {#equals_1}

Kontrollerar om detta objekt refererar till samma cell som ett annat.

```csharp
public override bool Equals(object obj)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | Object | annat objekt |

### Returvärde

true om två objekt refererar till samma cell.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Åtkomst till celler från olika platser
            Cell cellA1 = worksheet.Cells["A1"];
            Cell anotherCellA1 = worksheet.Cells[0, 0]; // Same physical cell as A1
            Cell cellB1 = worksheet.Cells["B1"];

            // Ange identiska värden i olika celler
            cellA1.PutValue("Aspose.Cells");
            cellB1.PutValue("Aspose.Cells");

            try
            {
                // Jämför samma fysiska cellreferenser
                bool sameCellComparison = cellA1.Equals(anotherCellA1);
                Console.WriteLine($"Same cell comparison: {sameCellComparison}"); // True

                // Jämför olika celler med identiskt innehåll
                bool differentCellComparison = cellA1.Equals(cellB1);
                Console.WriteLine($"Different cell comparison: {differentCellComparison}"); // False

                // Jämför cell med icke‑cellobjekt
                bool invalidTypeComparison = cellA1.Equals("Aspose.Cells");
                Console.WriteLine($"Invalid type comparison: {invalidTypeComparison}"); // False
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("CellMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Cell) {#equals}

Kontrollerar om detta objekt refererar till samma cell som ett annat cellobjekt.

```csharp
public bool Equals(Cell cell)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cell | Cell | ett annat cellobjekt |

### Returvärde

true om två cellobjekt refererar till samma cell.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithCellDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa celler på olika platser (A1 och B1)
            Cell cellA1 = worksheet.Cells[0, 0];
            Cell cellB1 = worksheet.Cells[0, 1];

            // Ange identiska värden i båda cellerna
            cellA1.Value = "Aspose.Cells Comparison";
            cellB1.Value = "Aspose.Cells Comparison";

            try
            {
                // Jämför cellA1 med cellB1 (olika platser)
                bool equalsResult = cellA1.Equals(cellB1);
                Console.WriteLine($"Cell A1 equals Cell B1: {equalsResult}");

                // Jämför cellA1 med sig själv (samma instans)
                equalsResult = cellA1.Equals(cellA1);
                Console.WriteLine($"Cell A1 equals itself: {equalsResult}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Spara arbetsboken
            workbook.Save("CellMethodEqualsWithCellDemo.xlsx");
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


