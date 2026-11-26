---
title: "Enumeración AutoFitWrappedTextType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.AutoFitWrappedTextType enum. Representa el tipo de ajuste automático de texto envuelto"
type: docs
url: /es/net/aspose.cells/autofitwrappedtexttype/
---
## AutoFitWrappedTextType enumeration

Representa el tipo de ajuste automático de texto ajustado.

```csharp
public enum AutoFitWrappedTextType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Default | `0` | Funciona como MS Excel. |
| Paragraph | `1` | Ajusta automáticamente el ancho con el párrafo más largo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitWrappedTextTypeDemo
    {
        public static void AutoFitWrappedTextTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("This is a sample text that will be wrapped and auto-fitted.\r\n This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted. This is a sample text that will be wrapped and auto-fitted.");
            worksheet.Cells["A5"].PutValue("Another sample text to demonstrate \r\n auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.\r\n Another sample text to demonstrate auto-fitting wrapped text. Another sample text to demonstrate auto-fitting wrapped text.");

            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            Style style2 = worksheet.Cells["A5"].GetStyle();
            style2.IsTextWrapped = true;
            worksheet.Cells["A5"].SetStyle(style);

            // Crea un rango A1:F3
            Range range = worksheet.Cells.CreateRange(0, 0, 3, 6);
            // Combina las celdas
            range.Merge();

            // Crea un rango A4:F6
            Range range2 = worksheet.Cells.CreateRange(4, 0, 3, 6);
            // Combina las celdas
            range2.Merge();

            // Crea AutoFitterOptions y establece AutoFitWrappedTextType
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph;

            // Ajusta automáticamente las filas con las opciones especificadas
            worksheet.AutoFitRows(options);

            // Guarda el libro de trabajo
            workbook.Save("AutoFitWrappedTextTypeExample.xlsx");
            workbook.Save("AutoFitWrappedTextTypeExample.pdf");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


