---
title: "FontFileDataInfo.FormatType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FontFileDataInfo-Eigenschaft. Gibt den Schriftformattyp der Schriftdatei zurück"
type: docs
url: /de/net/aspose.cells/fontfiledatainfo/formattype/
---
## FontFileDataInfo.FormatType property

Liest Schriftformattyp der Schriftdatei.

```csharp
public FontFileFormatType FormatType { get; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge etwas Text hinzu, um die Verwendung der Schriftart zu demonstrieren
            worksheet.Cells["A1"].PutValue("Sample Text with Font");

            try
            {
                // Lade eine Beispiel-Schriftdatei (ersetze durch den tatsächlichen Pfad zur Schriftdatei)
                string fontFilePath = "arial.ttf";
                if (File.Exists(fontFilePath))
                {
                    // Registriere den Schriftordner
                    FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);

                    // In einem echten Szenario würde FontFileDataInfo aus der Bibliothek bezogen werden
                    // Zur Demonstration simulieren wir das Abrufen von Schriftinformationen
                    // Hinweis: Die tatsächliche API könnte dies über FontConfigs oder Ähnliches bereitstellen
                    FontFileDataInfo fontInfo = GetFontFileDataInfo(fontFilePath);

                    if (fontInfo != null)
                    {
                        // Zeige den Wert der FormatType-Eigenschaft an
                        Console.WriteLine("Font Format Type: " + fontInfo.FormatType);

                        // Zeige den Enum-Wert als Zeichenkette
                        Console.WriteLine("Format Type Description: " +
                            Enum.GetName(typeof(FontFileFormatType), fontInfo.FormatType));

                        // Wende die Schriftart auf eine Zelle an (konzeptionell – die tatsächliche Implementierung kann variieren)
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

                // Speichere die Arbeitsmappe
                workbook.Save("FormatTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        // Hilfsmethode, um das Abrufen von FontFileDataInfo zu simulieren
        // Bei realer Verwendung würde dies von der Aspose.Cells API bereitgestellt werden
        private static FontFileDataInfo GetFontFileDataInfo(string fontPath)
        {
            try
            {
                byte[] fontData = File.ReadAllBytes(fontPath);
                string extension = Path.GetExtension(fontPath).ToLower();

                // Erstelle ein Mock-Objekt von FontFileDataInfo (in Wirklichkeit würde dies von der API kommen)
                // Da wir es nicht direkt instanziieren können, simulieren wir das Verhalten
                FontFileFormatType formatType = FontFileFormatType.Unknown;

                if (extension == ".ttf")
                    formatType = FontFileFormatType.Ttf;
                else if (extension == ".otf")
                    formatType = FontFileFormatType.Otf;
                else if (extension == ".ttc")
                    formatType = FontFileFormatType.Ttc;

                // In einer echten Implementierung würde dies von der API zurückgegeben werden
                // Für diese Demo geben wir einfach null zurück, da wir das Objekt nicht erstellen können
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

### Siehe auch

* enum [FontFileFormatType](../../fontfileformattype/)
* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


