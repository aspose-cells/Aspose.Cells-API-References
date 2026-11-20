---
title: "IExportObjectListener"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Consente agli utenti di manipolare gli oggetti durante l'esportazione."
type: docs
url: /it/java/com.aspose.cells/iexportobjectlistener/
---
```
public interface IExportObjectListener
```

Consente agli utenti di manipolare gli oggetti durante l'esportazione.

**Example**

Il seguente esempio crea un Workbook, apre un file chiamato designer.xls al suo interno e rende invisibili le barre di scorrimento orizzontali e verticali per il Workbook. Quindi sostituisce due valori stringa con un valore Integer e un valore stringa rispettivamente all'interno del foglio di calcolo e infine invia il file aggiornato al browser client.

```
             class CustomExportObjectListener implements IExportObjectListener
             {
                 private int imgIdx = 0;
                 public Object exportObject(ExportObjectEvent e)
                 {
                     Object source = e.getSource();
                     if (source instanceof Shape)
                     {
                         Shape shape = (Shape)source;
                         String url = null;
                         switch (shape.getMsoDrawingType())
                         {
                             case MsoDrawingType.PICTURE:
                             {
                                 url = saveImage(((Picture)shape).getData(), imgIdx, ((Picture)shape).getImageType());
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
                 private String saveImage(byte[] data, int imgIdx, /*ImageType*/int format)
                 {
                     //here save the image to any location, then return the url(relative or absolute) that the generated html can get the image
                     return "temp1/temp2.png";
                 }
              }
             //custom implementation of IExportObjectListener
 
                 //Save html file with custom listener
                 Workbook book = null; //build your workbook here
                 HtmlSaveOptions saveOptions = new HtmlSaveOptions();
                 saveOptions.setExportObjectListener(new CustomExportObjectListener());
                 java.io.InputStream stream = null; //build your stream here
                 book.save("res.html", saveOptions); //or here you can build your out put stream and save the workbook to stream
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [exportObject(ExportObjectEvent e)](#exportObject-com.aspose.cells.ExportObjectEvent-) | Esporta un oggetto. |
### exportObject(ExportObjectEvent e) {#exportObject-com.aspose.cells.ExportObjectEvent-}
```
public abstract Object exportObject(ExportObjectEvent e)
```


Esporta un oggetto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| e | [ExportObjectEvent](../../com.aspose.cells/exportobjectevent) | L'evento attivato quando un oggetto deve essere esportato. |

**Returns:**
java.lang.Object - Le informazioni sul risultato dell'esportazione dell'oggetto.

 *  For exporting objects when export workbook to HTML format, the result is URL string to access the saved Image from the html file which contains this exported object.
