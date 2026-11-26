---
title: "Range.ClearContents"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Borra el contenido de este rango"
type: docs
url: /es/net/aspose.cells/range/clearcontents/
---
## Range.ClearContents method

Borra el contenido de este rango.

```csharp
public void ClearContents()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearContentsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo para demostrar la limpieza
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            worksheet.Cells["A2"].PutValue("Sample");
            worksheet.Cells["B2"].PutValue("Data");

            try
            {
                // Crear un rango que cubra las celdas A1:B2
                Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B2");

                // Mostrar el contenido del rango antes de la limpieza
                Console.WriteLine("Before clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Llamar a ClearContents para eliminar todos los valores del rango
                range.ClearContents();

                // Mostrar el contenido del rango después de la limpieza
                Console.WriteLine("\nAfter clearing:");
                Console.WriteLine($"A1: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"B1: {worksheet.Cells["B1"].Value}");
                Console.WriteLine($"A2: {worksheet.Cells["A2"].Value}");
                Console.WriteLine($"B2: {worksheet.Cells["B2"].Value}");

                // Guarda el libro de trabajo
                workbook.Save("ClearContentsDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
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

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


