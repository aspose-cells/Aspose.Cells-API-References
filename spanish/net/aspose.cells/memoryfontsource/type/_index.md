---
title: "MemoryFontSource.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MemoryFontSource. Devuelve el tipo de la fuente"
type: docs
url: /es/net/aspose.cells/memoryfontsource/type/
---
## MemoryFontSource.Type property

Devuelve el tipo del origen de la fuente.

```csharp
public override FontSourceType Type { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            // Cargar un archivo de fuente TrueType en memoria
            byte[] fontData = File.ReadAllBytes("arial.ttf");

            // Crear una instancia de MemoryFontSource con los datos de la fuente
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);

            // Mostrar el valor actual de Type
            Console.WriteLine("MemoryFontSource Type: " + memoryFontSource.Type);

            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer fuentes usando FontConfigs
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Verificar que el tipo de fuente sea MemoryFont
            if (memoryFontSource.Type == FontSourceType.MemoryFont)
            {
                // Usar la fuente en una celda
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].PutValue("Text using memory font source");

                // Agregar información sobre el tipo de fuente
                worksheet.Cells["A2"].PutValue("Font source type: " + memoryFontSource.Type);
            }

            // Guarda el libro de trabajo
            workbook.Save("MemoryFontSourceTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FontSourceType](../../fontsourcetype/)
* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


