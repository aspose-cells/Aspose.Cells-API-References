---
title: "ConditionalFormattingIcon.GetIconImageData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ConditionalFormattingIcon-Methode. Gibt die Symbolsatzdaten zurück"
type: docs
url: /de/net/aspose.cells/conditionalformattingicon/geticonimagedata/
---
## ConditionalFormattingIcon.GetIconImageData method

Rufen Sie die Icon-Set-Daten ab

```csharp
public static byte[] GetIconImageData(IconSetType type, int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | IconSetType | Typ des Symbols |
| Index | Int32 | Index des Symbols |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class ConditionalFormattingIconMethodGetIconImageDataWithIconSetTypeInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Keine Instanz erforderlich, da GetIconImageData statisch ist
            
            try
            {
                // Rufen Sie GetIconImageData mit IconSetType.Arrows3 und Index 0 auf
                byte[] imageData = ConditionalFormattingIcon.GetIconImageData(IconSetType.Arrows3, 0);
                
                Console.WriteLine("Method executed successfully. Image data length: " + imageData.Length);
                
                // Speichern Sie die Bilddaten zu Demonstrationszwecken in einer Datei
                File.WriteAllBytes("icon_image.png", imageData);
                Console.WriteLine("Icon image saved to icon_image.png");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetIconImageData method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("ConditionalFormattingIconGetIconImageDataDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [IconSetType](../../iconsettype/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


