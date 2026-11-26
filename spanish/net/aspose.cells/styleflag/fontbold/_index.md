---
title: "StyleFlag.FontBold"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración de fuente en negrita"
type: docs
url: /es/net/aspose.cells/styleflag/fontbold/
---
## StyleFlag.FontBold property

Se aplicará la configuración de negrita de fuente.

```csharp
public bool FontBold { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontBoldDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo en negrita
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // Aplicar estilo en negrita a la fila 2 con StyleFlag solo para FontBold
            worksheet.Cells.ApplyRowStyle(1, boldStyle, new StyleFlag { FontBold = true });

            // Colocar valor en la celda para demostrar el estilo
            worksheet.Cells[1, 0].PutValue("Bold Text");

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            Console.WriteLine("FontBold property demo completed successfully.");
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


