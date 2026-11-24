---
title: "PageSetup.SetPicture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Setzt ein Bild in die Kopf-/Fußzeile eines Arbeitsblatts."
type: docs
url: /de/net/aspose.cells/pagesetup/setpicture/
---
## PageSetup.SetPicture method

Fügt ein Bild in die Kopf-/Fußzeile eines Arbeitsblatts ein.

```csharp
public Picture SetPicture(bool isFirst, bool isEven, bool isHeader, int section, byte[] imageData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isFirst | Boolean | Gibt an, ob das Bild der ersten Seite in der Kopf-/Fußzeile gesetzt wird. |
| isEven | Boolean | Gibt an, ob das Bild der geraden Seite in der Kopf-/Fußzeile gesetzt wird. |
| isHeader | Boolean | Gibt an, ob das Bild der Kopf-/Fußzeile gesetzt wird. |
| Abschnitt | Int32 | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt. |
| imageData | Byte[] | Bilddaten. |

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

    public class PageSetupMethodSetPictureWithBooleanBooleanBooleanInt32ByteDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Lade eine Bilddatei in ein Byte‑Array
            byte[] imageData = File.ReadAllBytes("example.jpg");

            try
            {
                // Rufe die SetPicture‑Methode auf, um das Kopfzeilenbild zu setzen
                // Parameter: isFirstPage, isEvenPage, isHeader, section, imageData
                Picture picture = pageSetup.SetPicture(false, false, true, 1, imageData);

                // Kopfzeilentext festlegen
                pageSetup.SetHeader(1, "&G");
                
                Console.WriteLine("SetPicture method executed successfully. Header image set.");

                // Speichere die Arbeitsmappe
                workbook.Save("PageSetupSetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetPicture method: {ex.Message}");
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


