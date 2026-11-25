---
title: "Class ExportObjectEvent"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ExportObjectEvent. L'evento attivato durante l'esportazione di un oggetto come Immagine"
type: docs
url: /it/net/aspose.cells/exportobjectevent/
---
## ExportObjectEvent class

L'evento attivato durante l'esportazione di un oggetto, come Picture.

```csharp
public class ExportObjectEvent
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetSource](../../aspose.cells/exportobjectevent/getsource/)() | Ottiene l'oggetto da esportare. |

### Esempi

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
            // Implementazione personalizzata di IExportObjectListener
            // Salva il file HTML con un listener personalizzato
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
            // Qui salva l'immagine in qualsiasi posizione, quindi restituisci l'URL (relativo o assoluto) che l'HTML generato può utilizzare per ottenere l'immagine
            return $"temp{imgIdx}/temp{imgIdx}.png";
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


