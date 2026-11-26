---
title: "UnionRange.Name"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad UnionRange. Obtiene o establece el nombre del rango"
type: docs
url: /es/net/aspose.cells/unionrange/name/
---
## UnionRange.Name property

Obtiene o establece el nombre del rango.

```csharp
public string Name { get; set; }
```

### Observaciones

Los rangos con nombre son compatibles. Por ejemplo,

range.Name = "Sheet1!MyRange";

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UnionRangePropertyNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].Value = "First Range";
            worksheet.Cells["B2"].Value = "Second Range";

            try
            {
                // Crea rangos y combínalos en un rango de unión
                Aspose.Cells.Range range1 = worksheet.Cells.CreateRange("A1:A1");
                Aspose.Cells.Range range2 = worksheet.Cells.CreateRange("B2:B2");
                UnionRange unionRange = (UnionRange)worksheet.Cells.Ranges.Union(new Aspose.Cells.Range[] { range1, range2 });

                // Mostrar el valor actual de la propiedad Name
                Console.WriteLine("Initial Name value: " + unionRange.Name);

                // Establecer un nuevo nombre para el rango de unión
                unionRange.Name = "MyUnionRange";
                Console.WriteLine("Updated Name value: " + unionRange.Name);

                // Demostrar que el nombre puede cambiarse nuevamente
                unionRange.Name = "CustomUnionRange";
                Console.WriteLine("Final Name value: " + unionRange.Name);

                // Guarda el libro de trabajo
                workbook.Save("UnionRangeNameDemo.xlsx");
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


