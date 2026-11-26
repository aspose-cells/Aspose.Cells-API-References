---
title: "FontFileDataInfo.Data"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontFileDataInfo. Obtiene los datos binarios del archivo de fuente"
type: docs
url: /es/net/aspose.cells/fontfiledatainfo/data/
---
## FontFileDataInfo.Data property

Obtiene los datos binarios del archivo de fuente.

```csharp
public byte[] Data { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyDataDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Cargar un archivo de fuente (reemplazar con la ruta real del archivo de fuente)
            string fontFilePath = "samplefont.ttf";
            byte[] fontData = File.ReadAllBytes(fontFilePath);

            // Crear una instancia de FontConfigs y agregar la fuente
            FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);
            
            // En uso real, FontFileDataInfo se obtendría de la biblioteca
            // Para fines de demostración, solo mostraremos cómo lo usarías si tuvieras uno
            FontFileDataInfo fontInfo = null; // Normally obtained from library APIs
            
            // Mostrar información sobre los datos de la fuente (si están disponibles)
            Console.WriteLine("Font data length: " + (fontInfo?.Data != null ? fontInfo.Data.Length.ToString() : "null"));
            if (fontInfo != null)
            {
                Console.WriteLine("Font format type: " + fontInfo.FormatType);
            }

            // En uso real, la propiedad Data se usaría para acceder a los datos binarios de la fuente
            // Por ejemplo, podrías guardarlo en un archivo:
            if (fontInfo?.Data != null && fontInfo.Data.Length > 0)
            {
                File.WriteAllBytes("extracted_font.ttf", fontInfo.Data);
                Console.WriteLine("Font data extracted to file.");
            }

            // Guardar el libro de trabajo (la fuente afectaría la representación si se usa en celdas)
            workbook.Save("FontDataDemo.xlsx");
        }
    }
}
```

### Ver también

* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


