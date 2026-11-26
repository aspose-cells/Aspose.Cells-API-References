---
title: "MemoryFontSource.MemoryFontSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor MemoryFontSource. Ctor"
type: docs
url: /es/net/aspose.cells/memoryfontsource/memoryfontsource/
---
## MemoryFontSource constructor

Ctor.

```csharp
public MemoryFontSource(byte[] fontData)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fontData | Byte[] | Datos binarios de la fuente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class MemoryFontSourceMethodCtorWithByteArrayDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            try
            {
                // Cargar un archivo de fuente TrueType en un arreglo de bytes
                byte[] fontData = File.ReadAllBytes("arial.ttf");
                
                // Llamar al método #ctor con un parámetro de arreglo de bytes
                MemoryFontSource fontSource = new MemoryFontSource(fontData);
                
                // Establecer fuentes usando la clase estática FontConfigs
                FontConfigs.SetFontSources(new FontSourceBase[] { fontSource });
                
                // Verificar las propiedades de la fuente
                Console.WriteLine($"Font source type: {fontSource.Type}");
                Console.WriteLine($"Font data length: {fontSource.FontData.Length} bytes");
                
                // Usar la fuente en una celda
                Worksheet worksheet = workbook.Worksheets[0];
                var style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                style.Font.Size = 14;
                worksheet.Cells["A1"].PutValue("Text with custom font");
                worksheet.Cells["A1"].SetStyle(style);
                
                Console.WriteLine("MemoryFontSource constructor executed successfully with byte array parameter");
            }
            catch (FileNotFoundException ex)
            {
                Console.WriteLine($"Error: Font file not found. {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing MemoryFontSource constructor: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("MemoryFontSourceCtorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


