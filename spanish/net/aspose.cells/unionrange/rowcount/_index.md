---
title: "UnionRange.RowCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad UnionRange. Obtiene el recuento de filas en el rango"
type: docs
url: /es/net/aspose.cells/unionrange/rowcount/
---
## UnionRange.RowCount property

Obtiene el recuento de filas en el rango.

```csharp
public int RowCount { get; }
```

### Observaciones

Solo tiene efecto cuando solo contiene un rango.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyRowCountDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Pobla datos en la hoja de cálculo
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].Value = $"Data {row},{col}";
                }
            }

            // Crear un rango de unión desde A1 hasta E5
            Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:E5");
            Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A6:E10");
            UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

            // Mostrar la propiedad RowCount
            Console.WriteLine("RowCount of union range: " + unionRange.RowCount);

            // Demostrar el uso iterando a través de filas
            for (int i = 0; i < unionRange.RowCount; i++)
            {
                Aspose.Cells.Range currentRow = worksheet.Cells.CreateRange(
                    unionRange.FirstRow + i,
                    unionRange.FirstColumn,
                    1,
                    unionRange.ColumnCount);

                Console.WriteLine($"Row {i + 1} first cell value: " + currentRow[0, 0].Value);
            }

            // Crear un nuevo rango con un recuento de filas diferente
            Aspose.Cells.Range newRange = worksheet.Cells.CreateRange("A1:E3");
            Console.WriteLine("RowCount of new range: " + newRange.RowCount);

            // Aplicar formato basado en el recuento de filas
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightYellow;
            style.Pattern = BackgroundType.Solid;

            for (int i = 0; i < unionRange.RowCount; i += 2)
            {
                Aspose.Cells.Range rowRange = worksheet.Cells.CreateRange(
                    unionRange.FirstRow + i,
                    unionRange.FirstColumn,
                    1,
                    unionRange.ColumnCount);
                rowRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });
            }

            // Guarda el libro de trabajo
            workbook.Save("UnionRangeRowCountDemo.xlsx");
        }
    }
}
```

### Ver también

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


