---
title: "MemoryFontSource.FontData"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MemoryFontSource. Datos binarios de la fuente"
type: docs
url: /es/net/aspose.cells/memoryfontsource/fontdata/
---
## MemoryFontSource.FontData property

Datos binarios de la fuente.

```csharp
public byte[] FontData { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourcePropertyFontDataDemo
    {
        public static void Run()
        {
            // Cargar un archivo de fuente TrueType en memoria
            byte[] fontBytes = File.ReadAllBytes("arial.ttf");

            // Crear una instancia de MemoryFontSource con los datos de la fuente
            MemoryFontSource memoryFontSource = new MemoryFontSource(fontBytes);

            // Mostrar el valor actual de FontData (primeros 10 bytes para demostración)
            Console.WriteLine("FontData length: " + memoryFontSource.FontData.Length);
            Console.Write("First 10 bytes: ");
            for (int i = 0; i < 10 && i < memoryFontSource.FontData.Length; i++)
            {
                Console.Write(memoryFontSource.FontData[i].ToString("X2") + " ");
            }
            Console.WriteLine();

            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear la configuración de fuentes y agregar nuestra fuente de memoria
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Aplicar la configuración de fuentes globalmente (no específica del libro de trabajo)
            FontConfigs.DefaultFontName = "Arial";
            FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });

            // Crear un estilo con la fuente personalizada
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;

            // Aplicar el estilo a una celda
            worksheet.Cells["A1"].SetStyle(style);
            worksheet.Cells["A1"].PutValue("Text using memory font source");

            // Guarda el libro de trabajo
            workbook.Save("MemoryFontSourceDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


