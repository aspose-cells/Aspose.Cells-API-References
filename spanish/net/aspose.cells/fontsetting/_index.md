---
title: "Clase FontSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.FontSetting. Representa un rango de caracteres dentro del texto de la celda"
type: docs
url: /es/net/aspose.cells/fontsetting/
---
## FontSetting class

Representa un rango de caracteres dentro del texto de la celda.

```csharp
public class FontSetting
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [FontSetting](fontsetting/)(int, int, WorksheetCollection) |  |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | Devuelve la fuente de este objeto. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | Obtiene la longitud de los caracteres. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | Obtiene el índice inicial de los caracteres. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | Devuelve las opciones de texto. |
| virtual [Type](../../aspose.cells/fontsetting/type/) { get; } | Obtiene el tipo de nodo de texto. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | Establece el estilo predefinido de WordArt. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class FontSettingDemo
    {
        public static void FontSettingExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();

            // Añadiendo una nueva hoja de cálculo al objeto Excel
            workbook.Worksheets.Add();

            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[0];

            // Accediendo a la celda "A1" de la hoja de cálculo
            Aspose.Cells.Cell cell = worksheet.Cells["A1"];

            // Añadiendo un valor a la celda "A1"
            cell.PutValue("Visit Aspose!");

            // Obteniendo rango de caracteres
            FontSetting character = cell.Characters(6, 7);

            // Estableciendo la fuente de los caracteres seleccionados en negrita
            character.Font.IsBold = true;

            // Estableciendo el color de fuente de los caracteres seleccionados en azul
            character.Font.Color = Color.Blue;

            // Guardando el archivo Excel
            workbook.Save("FontSettingExample.xlsx");
            workbook.Save("FontSettingExample.pdf");

        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


