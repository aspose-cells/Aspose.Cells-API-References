---
title: "Schnittstelle IExportObjectListener"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.IExportObjectListener Schnittstelle. Ermöglicht Benutzern, Objekte beim Export zu manipulieren"
type: docs
url: /de/net/aspose.cells/iexportobjectlistener/
---
## IExportObjectListener interface

Ermöglicht Benutzern, Objekte beim Exportieren zu manipulieren.

```csharp
public interface IExportObjectListener
```

## Methoden

| Name | Beschreibung |
| --- | --- |
| [ExportObject](../../aspose.cells/iexportobjectlistener/exportobject/)(ExportObjectEvent) | Exportiere ein Objekt. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CellsClassIExportObjectListenerDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge ein Beispielbild zum Arbeitsblatt hinzu.
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Benutzerdefinierte Export-Listener-Implementierung
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportObjectListener = new CustomExportObjectListener();
            
            // Speichere als HTML mit benutzerdefiniertem Listener
            workbook.Save("output.html", saveOptions);
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;
        
        public object ExportObject(ExportObjectEvent e)
        {
            object source = e.GetSource();
            if (source is Shape)
            {
                Shape shape = (Shape)source;
                if (shape.MsoDrawingType == MsoDrawingType.Picture)
                {
                    string url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
                    imgIdx++;
                    return url;
                }
            }
            return null;
        }
        
        private string SaveImage(byte[] data, int imgIdx, ImageType format)
        {
            // In einer echten Implementierung würdest du das Bild hier auf die Festplatte speichern
            // Zu Demonstrationszwecken geben wir einfach einen Dummy-Pfad zurück
            return $"images/image_{imgIdx}.png";
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


