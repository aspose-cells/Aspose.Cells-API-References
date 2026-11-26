---
title: "DefaultStyleSettings.VerticalAlignment"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DefaultStyleSettings. Gets/Sets el valor predeterminado para la alineación vertical"
type: docs
url: /es/net/aspose.cells/defaultstylesettings/verticalalignment/
---
## DefaultStyleSettings.VerticalAlignment property

Obtiene/Establece el valor predeterminado para la alineación vertical

```csharp
public TextAlignmentType VerticalAlignment { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Establezca la alineación vertical predeterminada a Inferior
            LoadOptions options = new LoadOptions();
            options.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer algunos datos de muestra
            worksheet.Cells["A1"].PutValue("Sample Text 1");
            worksheet.Cells["B1"].PutValue("Sample Text 2");
            worksheet.Cells["C1"].PutValue("Sample Text 3");

            // Verifique que la alineación vertical se aplique a todas las celdas
            foreach (Cell cell in worksheet.Cells)
            {
                Console.WriteLine($"Cell {cell.Name} Vertical Alignment: {cell.GetStyle().VerticalAlignment}");
            }

            // Guarda el libro de trabajo
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TextAlignmentType](../../textalignmenttype/)
* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


