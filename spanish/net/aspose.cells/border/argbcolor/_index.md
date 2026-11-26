---
title: "Border.ArgbColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Border. Obtiene y establece el color con un valor ARGB de 32 bits"
type: docs
url: /es/net/aspose.cells/border/argbcolor/
---
## Border.ArgbColor property

Obtiene y establece el color con un valor ARGB de 32 bits.

```csharp
public int ArgbColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyArgbColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a la celda B2 y establecer un valor
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Border ARGB Color Demo");

            // Obtener el estilo y los bordes
            Style style = cell.GetStyle();
            Border border = style.Borders[BorderType.TopBorder];

            // Establecer propiedades del borde incluyendo el color ARGB
            border.LineStyle = CellBorderType.Thick;
            unchecked
            {
                border.ArgbColor = (int)0xFFFF0000; // Red color in ARGB format with unchecked cast
            }

            // Aplicar el estilo modificado a la celda
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("BorderArgbColorDemo.xlsx");

            // Verificar que el color ARGB se haya establecido correctamente
            Border savedBorder = workbook.Worksheets[0].Cells["B2"].GetStyle().Borders[BorderType.TopBorder];
            Console.WriteLine("ARGB Color of top border: " + savedBorder.ArgbColor.ToString("X8"));
        }
    }
}
```

### Ver también

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


