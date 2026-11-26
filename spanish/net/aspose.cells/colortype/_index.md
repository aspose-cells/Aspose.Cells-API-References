---
title: "Enum ColorType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.ColorType. Representa todos los tipos de color"
type: docs
url: /es/net/aspose.cells/colortype/
---
## ColorType enumeration

Representa todos los tipos de color

```csharp
public enum ColorType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Automatic | `0` | Color automático. |
| AutomaticIndex | `1` | Es color automático, pero el color mostrado depende de la configuración del sistema operativo. |
| RGB | `2` | El color RGB. |
| IndexedColor | `3` | El índice de color en la paleta de colores. |
| Theme | `4` | El color del tema. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassColorTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Cree un nuevo libro de trabajo para la demostración
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Demostrar el uso de los valores del enum ColorType
                ColorType automatic = ColorType.Automatic;
                ColorType rgb = ColorType.RGB;
                ColorType theme = ColorType.Theme;

                // Mostrar los valores del enum
                Console.WriteLine($"Automatic color type value: {(int)automatic}");
                Console.WriteLine($"RGB color type value: {(int)rgb}");
                Console.WriteLine($"Theme color type value: {(int)theme}");

                // Crear una celda y establecer su valor
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ColorType Demo");

                // Crear un estilo y aplicarlo a la celda
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Black;
                cell.SetStyle(style);

                // Guarda el libro de trabajo
                workbook.Save("ColorTypeDemo.xlsx");

                Console.WriteLine("ColorType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ColorType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


