---
title: "Gränssnitt IExportObjectListener"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.IExportObjectListener-gränssnitt. Tillåter användare att manipulera objekt under export"
type: docs
url: /sv/net/aspose.cells/iexportobjectlistener/
---
## IExportObjectListener interface

Tillåter användare att manipulera objekt vid export.

```csharp
public interface IExportObjectListener
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [ExportObject](../../aspose.cells/iexportobjectlistener/exportobject/)(ExportObjectEvent) | Exportera ett objekt. |

### Exempel

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
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en exempelbild i kalkylbladet
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Anpassad exportlyssnare-implementation
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportObjectListener = new CustomExportObjectListener();
            
            // Spara till HTML med anpassad lyssnare
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
            // I en verklig implementation skulle du spara bilden till disk här
            // För demonstrationsändamål returnerar vi bara en dummy-sökväg
            return $"images/image_{imgIdx}.png";
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


