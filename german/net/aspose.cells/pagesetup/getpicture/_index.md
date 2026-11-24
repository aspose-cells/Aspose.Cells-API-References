---
title: "PageSetup.GetPicture"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Methode. Ruft das Picture-Objekt der Kopfzeile / Fußzeile ab."
type: docs
url: /de/net/aspose.cells/pagesetup/getpicture/
---
## GetPicture(bool, int) {#getpicture_1}

Ruft das [`Picture`](../../../aspose.cells.drawing/picture/)‑Objekt der Kopfzeile / Fußzeile ab.

```csharp
public Picture GetPicture(bool isHeader, int section)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isHeader | Boolean | Gibt an, ob es sich in der Kopfzeile oder Fußzeile befindet. |
| Abschnitt | Int32 | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt. |

### Rückgabewert

Gibt das [`Picture`](../../../aspose.cells.drawing/picture/)‑Objekt zurück. Gibt null zurück, wenn kein Bild vorhanden ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetPictureWithBooleanInt32Demo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge ein Bild zur Kopfzeile des Arbeitsblatts hinzu.
            byte[] imageData = System.IO.File.ReadAllBytes("header.png");
            worksheet.PageSetup.SetHeaderPicture(0, imageData);
            
            // Hole das Bild aus der Kopfzeile und ändere seine Helligkeit.
            Picture headerPicture = worksheet.PageSetup.GetPicture(true, 0);
            headerPicture.FormatPicture.Brightness = 50;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Picture](../../../aspose.cells.drawing/picture/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetPicture(bool, bool, bool, int) {#getpicture}

Ruft das [`Picture`](../../../aspose.cells.drawing/picture/)‑Objekt der Kopfzeile / Fußzeile ab.

```csharp
public Picture GetPicture(bool isFirst, bool isEven, bool isHeader, int section)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| isFirst | Boolean | Gibt an, ob das Bild der Kopf‑/Fußzeile der ersten Seite abgerufen wird. |
| isEven | Boolean | Gibt an, ob das Bild der Kopf‑/Fußzeile der geraden Seiten abgerufen wird. |
| isHeader | Boolean | Gibt an, ob das Bild der Kopf‑/Fußzeile abgerufen wird. |
| Abschnitt | Int32 | 0: Linker Abschnitt, 1: Mittlerer Abschnitt, 2: Rechter Abschnitt. |

### Rückgabewert

Gibt ein [`Picture`](../../../aspose.cells.drawing/picture/)‑Objekt zurück.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PageSetupMethodGetPictureWithBooleanBooleanBooleanInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Das PageSetup-Objekt abrufen
            PageSetup pageSetup = worksheet.PageSetup;
            
            // Setze einige Kopf‑/Fußzeilen‑Eigenschaften, um sicherzustellen, dass wir Bilder zum Abrufen haben.
            pageSetup.IsHFDiffFirst = true;
            pageSetup.IsHFDiffOddEven = true;
            
            try
            {
                // Rufe die GetPicture‑Methode mit den Parametern auf: isFirst, isEven, isHeader, section
                // Überprüfe die Kopfzeile der ersten Seite (Abschnitt 0 - mittlere Kopfzeile)
                Picture picture = pageSetup.GetPicture(true, false, true, 0);
                
                if (picture != null)
                {
                    Console.WriteLine("Retrieved picture from first page header:");
                    Console.WriteLine($"Original dimensions: {picture.OriginalWidth}x{picture.OriginalHeight}");
                }
                else
                {
                    Console.WriteLine("No picture found in first page header");
                }
                
                // Speichere die Arbeitsmappe
                workbook.Save("PageSetupGetPictureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetPicture method: {ex.Message}");
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


