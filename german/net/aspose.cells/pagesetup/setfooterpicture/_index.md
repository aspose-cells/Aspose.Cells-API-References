---
title: "PageSetup.SetFooterPicture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Legt ein Bild in der Fußzeile eines Arbeitsblatts fest"
type: docs
url: /de/net/aspose.cells/pagesetup/setfooterpicture/
---
## PageSetup.SetFooterPicture method

Fügt ein Bild in die Fußzeile eines Arbeitsblatts ein.

```csharp
public Picture SetFooterPicture(int section, byte[] footerPicture)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Abschnitt | Int32 | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt. |
| footerPicture | Byte[] | Bilddaten. |

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

    public class PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lade eine Bilddatei in ein Byte‑Array
            byte[] footerImageData = File.ReadAllBytes("footer_logo.png");
            
            try
            {
                // Rufen Sie die SetFooterPicture-Methode mit dem Abschnittsindex (0 für zentriert, 1 für links, 2 für rechts) und Bilddaten auf
                Picture footerPicture = worksheet.PageSetup.SetFooterPicture(0, footerImageData);
                
                // Setzen Sie den Fußzeilentext, um zusammen mit dem Bild angezeigt zu werden
                worksheet.PageSetup.SetFooter(0, "&G");
                
                Console.WriteLine("SetFooterPicture method executed successfully with parameters (Int32, Byte[])");
                
                // Speichern Sie die Arbeitsmappe, um das Fußzeilenbild zu sehen
                workbook.Save("PageSetupMethodSetFooterPictureWithInt32ByteArrayDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetFooterPicture method: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


