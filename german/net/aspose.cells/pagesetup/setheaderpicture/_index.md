---
title: "PageSetup.SetHeaderPicture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Legt ein Bild in der Kopfzeile eines Arbeitsblatts fest."
type: docs
url: /de/net/aspose.cells/pagesetup/setheaderpicture/
---
## PageSetup.SetHeaderPicture method

Fügt ein Bild in die Kopfzeile eines Arbeitsblatts ein.

```csharp
public Picture SetHeaderPicture(int section, byte[] headerPicture)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | Int32 | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt. |
| headerPicture | Byte[] | Bilddaten. |

### Rückgabewert

Gibt ein [`Picture`](../../../aspose.cells.drawing/picture/)‑Objekt zurück.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class PageSetupMethodSetHeaderPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lade eine Bilddatei in ein Byte‑Array
            byte[] headerImageBytes = File.ReadAllBytes("header_logo.png");
            
            try
            {
                // Rufen Sie SetHeaderPicture mit dem Abschnittsindex (0 für zentrierten Header) und Bildbytes auf
                Picture picture = worksheet.PageSetup.SetHeaderPicture(0, headerImageBytes);
                
                // Setzen Sie das Header-Skript, um das Bild anzuzeigen
                worksheet.PageSetup.SetHeader(0, "&G");
                
                Console.WriteLine("SetHeaderPicture method executed successfully with parameters (Int32, Byte[])");
                Console.WriteLine($"Picture dimensions: {picture.OriginalWidth}x{picture.OriginalHeight} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetHeaderPicture method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("SetHeaderPictureDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


