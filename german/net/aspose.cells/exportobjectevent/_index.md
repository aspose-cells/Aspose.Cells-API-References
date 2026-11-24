---
title: "Klasse ExportObjectEvent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExportObjectEvent Klasse. Das Ereignis, das ausgelöst wird, wenn ein Objekt wie ein Bild exportiert wird"
type: docs
url: /de/net/aspose.cells/exportobjectevent/
---
## ExportObjectEvent class

Das Ereignis, das beim Exportieren eines Objekts, wie z. B. Picture, ausgelöst wird.

```csharp
public class ExportObjectEvent
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [GetSource](../../aspose.cells/exportobjectevent/getsource/)() | Gibt das zu exportierende Objekt zurück. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ExportObjectEventDemo
    {
        public static void ExportObjectEventExample()
        {
            // Benutzerdefinierte Implementierung von IExportObjectListener
            // Speichere HTML-Datei mit benutzerdefiniertem Listener
            Workbook workbook = new Workbook(); // Build your workbook here
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = new CustomExportObjectListener()
            };
            using (Stream stream = new FileStream("ExportObjectEventExample.html", FileMode.Create))
            {
                workbook.Save(stream, saveOptions); // Save the workbook to stream
            }
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;

        public object ExportObject(ExportObjectEvent e)
        {
            object source = e.GetSource();
            if (source is Shape shape)
            {
                string url = null;
                switch (shape.MsoDrawingType)
                {
                    case MsoDrawingType.Picture:
                        url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
                        break;
                }
                if (url != null)
                {
                    imgIdx++;
                }
                return url;
            }
            return null;
        }

        private string SaveImage(byte[] data, int imgIdx, ImageType format)
        {
            // Hier wird das Bild an einem beliebigen Ort gespeichert und dann die URL (relativ oder absolut) zurückgegeben, die das erzeugte HTML zum Abrufen des Bildes verwenden kann
            return $"temp{imgIdx}/temp{imgIdx}.png";
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


