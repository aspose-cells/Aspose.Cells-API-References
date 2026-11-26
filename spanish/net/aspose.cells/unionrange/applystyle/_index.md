---
title: "UnionRange.ApplyStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método UnionRange. Aplica formatos para todo el rango"
type: docs
url: /es/net/aspose.cells/unionrange/applystyle/
---
## UnionRange.ApplyStyle method

Aplica formatos a todo un rango.

```csharp
public void ApplyStyle(Style style, StyleFlag flag)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | Estilo | El objeto de estilo que se aplicará. |
| bandera | StyleFlag | Banderas que indican las propiedades de formato aplicadas. |

### Observaciones

Cada celda en este rango contendrá un objeto [`Style`](../../style/). Por lo tanto, este es un método que consume mucha memoria. Por favor, úselo con cuidado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class UnionRangeMethodApplyStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un rango de unión que cubra las celdas A1 a B2
            UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });

            // Agregar algunos datos para contexto
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B2"].Value = "More Data";

            try
            {
                // Crea un estilo con formato específico
                Style style = workbook.CreateStyle();
                style.Font.IsBold = true;
                style.Font.Color = Color.Red;
                style.ForegroundColor = Color.LightBlue;
                style.Pattern = BackgroundType.Solid;
                style.HorizontalAlignment = TextAlignmentType.Center;

                // Crea un StyleFlag para especificar qué propiedades aplicar
                StyleFlag flag = new StyleFlag();
                flag.FontBold = true;
                flag.FontColor = true;
                flag.CellShading = true;
                flag.HorizontalAlignment = true;

                // Llama a ApplyStyle con los parámetros de estilo y bandera
                unionRange.ApplyStyle(style, flag);

                Console.WriteLine("ApplyStyle method called successfully");
                Console.WriteLine($"Applied style to range: {unionRange.RefersTo}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling ApplyStyle: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("UnionRangeMethodApplyStyleWithStyleStyleFlagDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


