---
title: "Clase MemoryFontSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.MemoryFontSource. Representa el único archivo de fuente TrueType almacenado en memoria"
type: docs
url: /es/net/aspose.cells/memoryfontsource/
---
## MemoryFontSource class

Representa el archivo de fuente TrueType único almacenado en memoria.

```csharp
public class MemoryFontSource : FontSourceBase
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [MemoryFontSource](memoryfontsource/)(byte[]) | Ctor. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FontData](../../aspose.cells/memoryfontsource/fontdata/) { get; } | Datos binarios de la fuente. |
| override [Type](../../aspose.cells/memoryfontsource/type/) { get; } | Devuelve el tipo del origen de la fuente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class CellsClassMemoryFontSourceDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Cargar un archivo de fuente TrueType en memoria
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Crear una instancia de MemoryFontSource con los datos de la fuente
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Crear una matriz de fuentes que contenga nuestra MemoryFontSource
            FontSourceBase[] fontSources = new FontSourceBase[] { memoryFontSource };

            // Establecer las fuentes usando FontConfigs
            FontConfigs.SetFontSources(fontSources);

            // Usar la fuente personalizada en una celda
            worksheet.Cells["A1"].PutValue("Text with custom font from memory");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            worksheet.Cells["A1"].SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


