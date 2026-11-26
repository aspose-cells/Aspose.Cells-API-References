---
title: "Clase FileFontSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.FileFontSource. Representa el único archivo de fuente TrueType almacenado en el sistema de archivos"
type: docs
url: /es/net/aspose.cells/filefontsource/
---
## FileFontSource class

Representa el único archivo de fuente TrueType almacenado en el sistema de archivos.

```csharp
public class FileFontSource : FontSourceBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [FileFontSource](filefontsource/)(string) | Ctor. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FilePath](../../aspose.cells/filefontsource/filepath/) { get; } | Ruta al archivo de fuente. |
| override [Type](../../aspose.cells/filefontsource/type/) { get; } | Devuelve el tipo del origen de la fuente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FileFontSourceDemo
    {
        public static void FileFontSourceExample()
        {
            // Especifique la ruta al archivo de fuente TrueType
            string fontFilePath = "C:\\Fonts\\CustomFont.ttf";

            // Crear una instancia de FileFontSource
            FileFontSource fontSource = new FileFontSource(fontFilePath);

            // Mostrar el tipo de origen de fuente y la ruta del archivo
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            Console.WriteLine("Font File Path: " + fontSource.FilePath);

            // Crear un objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Establecer un valor de celda
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Hello, Aspose!");

            // Aplicar la fuente personalizada a la celda
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont"; // Use the name of the font
            cell.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("FileFontSourceExample.xlsx");
            workbook.Save("FileFontSourceExample.pdf");
        }
    }
}
```

### Ver también

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


