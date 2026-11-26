---
title: "FontSourceBase.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontSourceBase. Devuelve el tipo de la fuente"
type: docs
url: /es/net/aspose.cells/fontsourcebase/type/
---
## FontSourceBase.Type property

Devuelve el tipo del origen de la fuente.

```csharp
public abstract FontSourceType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontSourceBasePropertyTypeDemo
    {
        public static void Run()
        {
            // Crear una instancia de libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear una fuente tipográfica de carpeta
            FolderFontSource folderFontSource = new FolderFontSource("C:\\MyFonts", true);
            
            // Mostrar la propiedad Type de la fuente
            Console.WriteLine("Font source type: " + folderFontSource.Type);
            
            // Crear una fuente de archivo
            FileFontSource fileFontSource = new FileFontSource("arial.ttf");
            
            // Mostrar la propiedad Type de la fuente
            Console.WriteLine("Font source type: " + fileFontSource.Type);
            
            // Crear una fuente de memoria (ejemplo con matriz de bytes)
            byte[] fontData = System.IO.File.ReadAllBytes("arial.ttf");
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);
            
            // Mostrar la propiedad Type de la fuente
            Console.WriteLine("Font source type: " + memoryFontSource.Type);
            
            // Establecer fuentes usando el método estático
            FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource, fileFontSource, memoryFontSource });
            
            // Guarda el libro de trabajo
            workbook.Save("FontSourceTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FontSourceType](../../fontsourcetype/)
* class [FontSourceBase](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


