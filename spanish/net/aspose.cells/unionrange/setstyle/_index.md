---
title: "UnionRange.SetStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método UnionRange. Establece el estilo del rango"
type: docs
url: /es/net/aspose.cells/unionrange/setstyle/
---
## UnionRange.SetStyle method

Establece el estilo del rango.

```csharp
public void SetStyle(Style style)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | El objeto Style. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos de ejemplo en el rango A1:B2
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["B1"].PutValue(123);
            worksheet.Cells["A2"].PutValue("Total");
            worksheet.Cells["B2"].PutValue(456);

            // Crear un UnionRange que cubra las celdas A1:B2
            UnionRange unionRange = worksheet.Cells
                .CreateRange("A1:B2")
                .UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            try
            {
                // Crear una instancia de Style y establecer algo de formato
                Style style = new Style();
                style.BackgroundColor = Color.LightYellow;
                style.ForegroundColor = Color.DarkBlue;
                style.HorizontalAlignment = TextAlignmentType.Center;
                style.VerticalAlignment = TextAlignmentType.Center;
                style.IsTextWrapped = true;

                // Aplicar el estilo al UnionRange
                unionRange.SetStyle(style);

                Console.WriteLine("SetStyle executed successfully on the UnionRange.");

                // Guardar el libro de trabajo para visualizar el resultado
                workbook.Save("UnionRangeSetStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetStyle: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


