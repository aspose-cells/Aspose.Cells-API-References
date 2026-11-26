---
title: "StyleFlag.Indent"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad StyleFlag. Se aplicará la configuración del nivel de sangría"
type: docs
url: /es/net/aspose.cells/styleflag/indent/
---
## StyleFlag.Indent property

Se aplicará la configuración de nivel de sangría.

```csharp
public bool Indent { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyIndentDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un estilo con nivel de sangría
            Style style = workbook.CreateStyle();
            style.IndentLevel = 2;
            style.HorizontalAlignment = TextAlignmentType.Left;

            // Crear bandera de estilo con la propiedad Indent establecida
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Indent = true;

            // Aplicar datos a las celdas
            for (int row = 0; row < 5; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    worksheet.Cells[row, col].PutValue($"Cell {row},{col}");
                }
            }

            // Aplicar el estilo con sangría a un rango
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 0, 5, 5);
            range.ApplyStyle(style, styleFlag);

            // Verificar que se aplicó el estilo
            Cell cell = worksheet.Cells["A1"];
            Style appliedStyle = cell.GetStyle();
            Console.WriteLine($"Indent Level: {appliedStyle.IndentLevel}");
            Console.WriteLine($"Alignment: {appliedStyle.HorizontalAlignment}");

            // Guarda el libro de trabajo
            workbook.Save("IndentStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


