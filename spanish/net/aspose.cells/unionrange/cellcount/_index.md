---
title: "UnionRange.CellCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad UnionRange. Obtiene el recuento total de celdas en el rango"
type: docs
url: /es/net/aspose.cells/unionrange/cellcount/
---
## UnionRange.CellCount property

Obtiene el recuento total de celdas en el rango.

```csharp
public int CellCount { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyCellCountDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pobla datos en la hoja de cálculo
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Cell {row + 1},{col + 1}";
                }
            }

            // Crea rangos y combínalos en un rango de unión
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:B3");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("D1:E4");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Muestra la propiedad CellCount
            Console.WriteLine("Total cells in union range: " + unionRange.CellCount);

            // Calcula el recuento de celdas esperado
            int expectedCount = (range1.RowCount * range1.ColumnCount) + (range2.RowCount * range2.ColumnCount);
            Console.WriteLine("Expected cell count: " + expectedCount);

            // Demuestra el uso iterando a través de las celdas
            Console.WriteLine("\nCell values in the union range:");
            int cellCounter = 0;
            foreach (Cell cell in unionRange)
            {
                Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                cellCounter++;
            }

            // Verifica que el recuento de celdas coincida con la iteración
            Console.WriteLine($"\nIterated through {cellCounter} cells (should match CellCount)");

            // Crea otro rango de unión con dimensiones diferentes
            Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("A5:E5");
            Aspose.Cells.Range range4 = worksheet.Cells.CreateRange("C1:C5");
            UnionRange unionRange2 = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range3, range4 });

            // Comparar recuentos de celdas de diferentes rangos de unión
            Console.WriteLine("\nSecond union range cell count: " + unionRange2.CellCount);
            Console.WriteLine("First union range has " + 
                (unionRange.CellCount > unionRange2.CellCount ? "more" : "fewer") + 
                " cells than second union range");

            // Guarda el libro de trabajo
            workbook.Save("UnionRangeCellCountDemo.xlsx");
        }
    }
}
```

### Ver también

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


