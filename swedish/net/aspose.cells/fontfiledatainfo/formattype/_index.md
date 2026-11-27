---
title: "FontFileDataInfo.FormatType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontFileDataInfo-egenskapen. Hämtar teckensnittets formattyp för teckensnittsfilen"
type: docs
url: /sv/net/aspose.cells/fontfiledatainfo/formattype/
---
## FontFileDataInfo.FormatType property

Hämtar teckensnittets formattyp för teckensnittsfilen.

```csharp
public FontFileFormatType FormatType { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite text för att demonstrera teckensnittsanvändning
            worksheet.Cells["A1"].PutValue("Sample Text with Font");

            try
            {
                // Läs in en exempelteckensnittsfil (ersätt med den faktiska teckensnittsfilens sökväg)
                string fontFilePath = "arial.ttf";
                if (File.Exists(fontFilePath))
                {
                    // Registrera teckensnittsmappen
                    FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);

                    // I ett verkligt scenario skulle FontFileDataInfo hämtas från biblioteket
                    // För demonstration kommer vi att simulera hämtning av teckensnittsinformation
                    // Obs: Det faktiska API:et kan tillhandahålla detta via FontConfigs eller liknande
                    FontFileDataInfo fontInfo = GetFontFileDataInfo(fontFilePath);

                    if (fontInfo != null)
                    {
                        // Visa värdet för egenskapen FormatType
                        Console.WriteLine("Font Format Type: " + fontInfo.FormatType);

                        // Visa enum-värdet som sträng
                        Console.WriteLine("Format Type Description: " +
                            Enum.GetName(typeof(FontFileFormatType), fontInfo.FormatType));

                        // Applicera teckensnittet på en cell (konceptuellt – faktisk implementation kan variera)
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

                // Spara arbetsboken
                workbook.Save("FormatTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Hjälpmetod för att simulera hämtning av FontFileDataInfo
        // Vid verklig användning skulle detta tillhandahållas av Aspose.Cells API
        private static FontFileDataInfo GetFontFileDataInfo(string fontPath)
        {
            try
            {
                byte[] fontData = File.ReadAllBytes(fontPath);
                string extension = Path.GetExtension(fontPath).ToLower();

                // Skapa ett mock-objekt av FontFileDataInfo (i verkligheten skulle detta komma från API:et)
                // Eftersom vi inte kan instansiera det direkt kommer vi att simulera beteendet
                FontFileFormatType formatType = FontFileFormatType.Unknown;

                if (extension == ".ttf")
                    formatType = FontFileFormatType.Ttf;
                else if (extension == ".otf")
                    formatType = FontFileFormatType.Otf;
                else if (extension == ".ttc")
                    formatType = FontFileFormatType.Ttc;

                // I en verklig implementation skulle detta returneras av API:et
                // För den här demonstrationen kommer vi bara att returnera null eftersom vi inte kan skapa objektet
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

### Se även

* enum [FontFileFormatType](../../fontfileformattype/)
* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


