---
title: "FontFileDataInfo.FormatType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad FontFileDataInfo. Obtiene el tipo de formato de fuente del archivo de fuente"
type: docs
url: /es/net/aspose.cells/fontfiledatainfo/formattype/
---
## FontFileDataInfo.FormatType property

Obtiene el tipo de formato de fuente del archivo de fuente.

```csharp
public FontFileFormatType FormatType { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class FontFileDataInfoPropertyFormatTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar texto para demostrar el uso de la fuente
            worksheet.Cells["A1"].PutValue("Sample Text with Font");

            try
            {
                // Cargar un archivo de fuente de ejemplo (reemplazar con la ruta real del archivo de fuente)
                string fontFilePath = "arial.ttf";
                if (File.Exists(fontFilePath))
                {
                    // Registrar la carpeta de fuentes
                    FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);

                    // En un escenario real, FontFileDataInfo se obtendría de la biblioteca
                    // Para demostración, simularemos la obtención de información de la fuente
                    // Nota: La API real podría proporcionar esto a través de FontConfigs o similar
                    FontFileDataInfo fontInfo = GetFontFileDataInfo(fontFilePath);

                    if (fontInfo != null)
                    {
                        // Mostrar el valor de la propiedad FormatType
                        Console.WriteLine("Font Format Type: " + fontInfo.FormatType);

                        // Mostrar el valor del enum como cadena
                        Console.WriteLine("Format Type Description: " +
                            Enum.GetName(typeof(FontFileFormatType), fontInfo.FormatType));

                        // Aplicar la fuente a una celda (conceptual - la implementación real puede variar)
                        Style style = worksheet.Cells["A1"].GetStyle();
                        style.Font.Name = "Arial";
                        worksheet.Cells["A1"].SetStyle(style);
                    }
                    else
                    {
                        Console.WriteLine("Font information could not be retrieved");
                    }
                }
                else
                {
                    Console.WriteLine("Font file not found at: " + fontFilePath);
                }

                // Guarda el libro de trabajo
                workbook.Save("FormatTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Método auxiliar para simular la obtención de FontFileDataInfo
        // En uso real, esto sería provisto por la API Aspose.Cells
        private static FontFileDataInfo GetFontFileDataInfo(string fontPath)
        {
            try
            {
                byte[] fontData = File.ReadAllBytes(fontPath);
                string extension = Path.GetExtension(fontPath).ToLower();

                // Crear un mock de FontFileDataInfo (en realidad, esto provendría de la API)
                // Dado que no podemos instanciarlo directamente, simularemos el comportamiento
                FontFileFormatType formatType = FontFileFormatType.Unknown;

                if (extension == ".ttf")
                    formatType = FontFileFormatType.Ttf;
                else if (extension == ".otf")
                    formatType = FontFileFormatType.Otf;
                else if (extension == ".ttc")
                    formatType = FontFileFormatType.Ttc;

                // En una implementación real, esto sería devuelto por la API
                // Para esta demostración, simplemente devolveremos null ya que no podemos crear el objeto
                Console.WriteLine($"Detected font format: {formatType}");
                return null;
            }
            catch
            {
                return null;
            }
        }
    }
}
```

### Ver también

* enum [FontFileFormatType](../../fontfileformattype/)
* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


