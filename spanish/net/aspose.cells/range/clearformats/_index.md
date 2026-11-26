---
title: "Range.ClearFormats"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Range. Elimina los formatos de este rango"
type: docs
url: /es/net/aspose.cells/range/clearformats/
---
## Range.ClearFormats method

Borra los formatos de este rango.

```csharp
public void ClearFormats()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangeMethodClearFormatsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega algunos datos con formato
            Cell cell = worksheet.Cells["A1"];
            cell.Value = "Formatted Cell";
            cell.GetStyle().Font.IsBold = true;
            cell.GetStyle().ForegroundColor = System.Drawing.Color.Yellow;
            cell.GetStyle().Pattern = BackgroundType.Solid;

            // Cree un rango
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:B5");

            try
            {
                // Elimina los formatos del rango
                range.ClearFormats();

                Console.WriteLine("Formats cleared successfully from range A1:B5");
                Console.WriteLine($"Cell A1 value after clearing formats: {worksheet.Cells["A1"].Value}");
                Console.WriteLine($"Cell A1 is bold after clearing formats: {worksheet.Cells["A1"].GetStyle().Font.IsBold}");

                // Guarda el libro de trabajo
                workbook.Save("ClearFormatsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ClearFormats: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


