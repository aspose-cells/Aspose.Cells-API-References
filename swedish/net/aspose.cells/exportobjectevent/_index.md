---
title: "Klass ExportObjectEvent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExportObjectEvent class. Händelsen som utlöses när ett objekt som Bild exporteras"
type: docs
url: /sv/net/aspose.cells/exportobjectevent/
---
## ExportObjectEvent class

Händelsen som utlöses när ett objekt exporteras, till exempel Bild.

```csharp
public class ExportObjectEvent
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetSource](../../aspose.cells/exportobjectevent/getsource/)() | Hämtar objektet som ska exporteras. |

### Exempel

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
            // Anpassad implementation av IExportObjectListener
            // Spara HTML-fil med anpassad lyssnare
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
            // Spara bilden här till valfri plats, returnera sedan URL:en (relativ eller absolut) som den genererade HTML‑koden kan hämta bilden
            return $"temp{imgIdx}/temp{imgIdx}.png";
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


