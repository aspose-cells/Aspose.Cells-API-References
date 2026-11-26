---
title: "Enum FontSourceType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.FontSourceType. Especifica el tipo de una fuente."
type: docs
url: /es/net/aspose.cells/fontsourcetype/
---
## FontSourceType enumeration

Especifica el tipo de origen de la fuente.

```csharp
public enum FontSourceType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| FontFile | `0` | representa un único archivo de fuente. |
| FontsFolder | `1` | Representa una carpeta con archivos de fuentes. |
| MemoryFont | `2` | Representa una única fuente en memoria. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassFontSourceTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Demostrar los valores del enum FontSourceType
            Console.WriteLine("FontSourceType values:");
            Console.WriteLine($"FontFile: {FontSourceType.FontFile}");
            Console.WriteLine($"FontsFolder: {FontSourceType.FontsFolder}");
            Console.WriteLine($"MemoryFont: {FontSourceType.MemoryFont}");

            // Crear configuraciones de fuente y usar FontSourceType
            FontConfigs.SetFontFolder(@"C:\MyFonts\", false);
            FontConfigs.SetFontSources(new FontSourceBase[]
            {
                new FolderFontSource(@"C:\MyFonts\", false),
                new FileFontSource(@"C:\MyFonts\arial.ttf"),
                new MemoryFontSource(new byte[0])
            });

            // Aplicar fuente a una celda
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text with Arial font");

            // Guardar el resultado
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


