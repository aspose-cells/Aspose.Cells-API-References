---
title: "ExportObjectEvent.GetSource"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ExportObjectEvent‑Methode. Liefert das zu exportierende Objekt"
type: docs
url: /de/net/aspose.cells/exportobjectevent/getsource/
---
## ExportObjectEvent.GetSource method

Gibt das zu exportierende Objekt zurück.

```csharp
public object GetSource()
```

### Rückgabewert

das zu exportierende Objekt.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ExportObjectEventMethodGetSourceDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Bild hinzu, um die GetSource‑Funktionalität zu demonstrieren
            int pictureIndex = worksheet.Pictures.Add(1, 1, "sample.jpg");
            Picture picture = worksheet.Pictures[pictureIndex];

            try
            {
                // Erstellen Sie einen benutzerdefinierten ExportObjectListener
                HtmlSaveOptions saveOptions = new HtmlSaveOptions
                {
                    ExportObjectListener = new CustomExportObjectListener()
                };

                // Speichere die Arbeitsmappe, um das ExportObjectEvent auszulösen
                using (Stream stream = new FileStream("GetSourceDemo.html", FileMode.Create))
                {
                    workbook.Save(stream, saveOptions);
                }

                Console.WriteLine("GetSource method demonstrated successfully. Check the output HTML file.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating GetSource: {ex.Message}");
            }
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        public object ExportObject(ExportObjectEvent e)
        {
            // Demonstriere die GetSource‑Methode
            object source = e.GetSource();

            if (source is Picture)
            {
                Console.WriteLine("GetSource returned a Picture object");
                return "custom-image-url.jpg";
            }

            return null;
        }
    }
}
```

### Siehe auch

* class [ExportObjectEvent](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


