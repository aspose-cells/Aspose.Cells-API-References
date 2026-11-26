---
title: "CellsHelper.GetUsedColors"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CellsHelper. Obtiene todos los colores usados en el libro de trabajo"
type: docs
url: /es/net/aspose.cells/cellshelper/getusedcolors/
---
## CellsHelper.GetUsedColors method

Obtiene todos los colores usados en el libro de trabajo.

```csharp
public static Color[] GetUsedColors(Workbook workbook)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| libro de trabajo | Libro de trabajo | El objeto libro de trabajo. |

### Valor de retorno

Los colores usados.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsHelperMethodGetUsedColorsWithWorkbookDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue algunas celdas coloreadas para demostrar los colores usados
            worksheet.Cells["A1"].PutValue("Red Cell");
            worksheet.Cells["A1"].GetStyle().ForegroundColor = Color.Red;
            worksheet.Cells["A1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["A1"].SetStyle(worksheet.Cells["A1"].GetStyle());

            worksheet.Cells["B1"].PutValue("Blue Cell");
            worksheet.Cells["B1"].GetStyle().ForegroundColor = Color.Blue;
            worksheet.Cells["B1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["B1"].SetStyle(worksheet.Cells["B1"].GetStyle());

            worksheet.Cells["C1"].PutValue("Green Cell");
            worksheet.Cells["C1"].GetStyle().ForegroundColor = Color.Green;
            worksheet.Cells["C1"].GetStyle().Pattern = BackgroundType.Solid;
            worksheet.Cells["C1"].SetStyle(worksheet.Cells["C1"].GetStyle());

            try
            {
                // Llame al método GetUsedColors con el parámetro libro de trabajo
                Color[] usedColors = CellsHelper.GetUsedColors(workbook);

                // Mostrar los colores usados
                Console.WriteLine("Used colors in the workbook:");
                foreach (Color color in usedColors)
                {
                    Console.WriteLine($"Color: A={color.A}, R={color.R}, G={color.G}, B={color.B}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetUsedColors method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("CellsHelperGetUsedColorsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Workbook](../../workbook/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


