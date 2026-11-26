---
title: "Clase ThemeColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ThemeColor. Representa un color de tema"
type: docs
url: /es/net/aspose.cells/themecolor/
---
## ThemeColor class

Representa un color de tema.

```csharp
public class ThemeColor
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ThemeColor](themecolor/)(ThemeColorType, double) |  |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ColorType](../../aspose.cells/themecolor/colortype/) { get; set; } | Obtiene y establece el tipo de tema. |
| [Tint](../../aspose.cells/themecolor/tint/) { get; set; } | Obtiene y establece el valor de tono. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorDemo
    {
        public static void ThemeColorExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Agregar un valor a la celda A1
            cells["A1"].PutValue("Hello World");

            // Obtener el estilo de la celda A1
            Style style = cells["A1"].GetStyle();

            // Establecer el tipo de color ThemeColorType.Text2 con un aclarado del 40% como color de fuente.
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text2, 0.4);
            style.Pattern = BackgroundType.Solid;

            // Establecer el tipo de color ThemeColorType.Background2 con un oscurecimiento del 75% como color de primer plano.
            style.ForegroundThemeColor = new ThemeColor(ThemeColorType.Background2, -0.75);

            // Aplicar el estilo a la celda A1
            cells["A1"].SetStyle(style);

            // Guardando el archivo Excel
            workbook.Save("ThemeColorExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


