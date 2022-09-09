---
title: IExportObjectListener
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Consente agli utenti di manipolare oggetti durante lesportazione.
type: docs
weight: 3790
url: /it/net/aspose.cells/iexportobjectlistener/
---
## IExportObjectListener interface

Consente agli utenti di manipolare oggetti durante l'esportazione.

```csharp
public interface IExportObjectListener
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ExportObject](../../aspose.cells/iexportobjectlistener/exportobject)(ExportObjectEvent) | Esporta un oggetto. |

### Esempi

L'esempio seguente crea una cartella di lavoro, apre un file denominato designer.xls al suo interno e rende invisibili le barre di scorrimento orizzontale e verticale per la cartella di lavoro. Quindi sostituisce due valori di stringa rispettivamente con un valore intero e un valore di stringa all'interno del foglio di calcolo e infine invia il file aggiornato al browser del client.

```csharp
[C#]
    //implementazione personalizzata di IExportObjectListener
    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;
        public object ExportObject(ExportObjectEvent e)
        {
            Object source = e.GetSource();
            if (source is Shape)
            {
                Shape shape = (Shape)source;
                string url = null;
                switch (shape.MsoDrawingType)
                {
                    case MsoDrawingType.Picture:
                    {
                        url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageFormat);
                        break;
                     }
                }
                if (url != null)
                {
                    imgIdx++;
                }
                return url;
            }
            return null;
        }
        private string SaveImage(byte[] data, int imgIdx, ImageFormat format)
        {
            //qui salva l'immagine in qualsiasi posizione, quindi restituisce l'URL (relativo o assoluto) che l'html generato può ottenere l'immagine
            return "temp1/temp2.png";
        }
     }
     
     //Salva il file html con il listener personalizzato
        HtmlSaveOptions saveOptions = new HtmlSaveOptions();
        saveOptions.ExportObjectListener = new CustomExportObjectListener();
        Stream stream = File.Create(outfn);
        book.Save(stream, saveOptions);
        stream.Flush();
        stream.Close();

```

### Guarda anche

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->