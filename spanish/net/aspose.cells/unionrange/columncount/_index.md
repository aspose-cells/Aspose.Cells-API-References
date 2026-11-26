---
title: "UnionRange.ColumnCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad UnionRange. Obtiene el recuento de filas en el rango"
type: docs
url: /es/net/aspose.cells/unionrange/columncount/
---
## UnionRange.ColumnCount property

Obtiene el recuento de filas en el rango.

```csharp
public int ColumnCount { get; }
```

### Observaciones

Solo tiene efecto cuando solo contiene un rango.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyColumnCountDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["C1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Laptop";
            worksheet.Cells["B2"].Value = 1200;
            worksheet.Cells["C2"].Value = 5;
            worksheet.Cells["A3"].Value = "Phone";
            worksheet.Cells["B3"].Value = 800;
            worksheet.Cells["C3"].Value = 10;

            try
            {
                // Crea rangos y combínalos en un rango de unión
                Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:C2");
                Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("A3:C3");
                UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

                // Mostrar el valor de la propiedad ColumnCount
                Console.WriteLine("ColumnCount of union range: " + unionRange.ColumnCount);

                // Demostrar el uso mostrando información de columnas
                Console.WriteLine("First column index: " + unionRange.FirstColumn);
                Console.WriteLine("Last column index: " + (unionRange.FirstColumn + unionRange.ColumnCount - 1));

                // Crear otro rango de unión con un recuento de columnas diferente
                Aspose.Cells.Range range3 = worksheet.Cells.CreateRange("A1:B2");
                Aspose.Cells.Range range4 = worksheet.Cells.CreateRange("D1:E2");
                UnionRange unionRange2 = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range3, range4 });

                // Comparar recuentos de columnas
                Console.WriteLine("Second union range ColumnCount: " + unionRange2.ColumnCount);
                Console.WriteLine("First union range has " +
                    (unionRange.ColumnCount > unionRange2.ColumnCount ? "more" : "fewer") +
                    " columns than second union range");

                // Guarda el libro de trabajo
                workbook.Save("UnionRangeColumnCountDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


