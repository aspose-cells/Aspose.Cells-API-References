---
title: "Interfaccia IExportObjectListener"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.IExportObjectListener interfaccia. Consente agli utenti di manipolare gli oggetti durante l'esportazione"
type: docs
url: /it/net/aspose.cells/iexportobjectlistener/
---
## IExportObjectListener interface

Consente agli utenti di manipolare gli oggetti durante l'esportazione.

```csharp
public interface IExportObjectListener
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ExportObject](../../aspose.cells/iexportobjectlistener/exportobject/)(ExportObjectEvent) | Esporta un oggetto. |

### Esempi

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
            // Crea una cartella di lavoro con dati di esempio
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi un'immagine di esempio al foglio di lavoro
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // Implementazione personalizzata del listener di esportazione
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportObjectListener = new CustomExportObjectListener();
            
            // Salva in HTML con listener personalizzato
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
            // In una reale implementazione, qui salveresti l'immagine su disco
            // Per scopi dimostrativi, restituiamo semplicemente un percorso fittizio
            return $"images/image_{imgIdx}.png";
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


