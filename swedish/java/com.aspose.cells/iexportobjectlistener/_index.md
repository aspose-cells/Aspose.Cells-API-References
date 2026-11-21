---
title: "IExportObjectListener"
second_title: "Aspose.Cells för Java API-referens"
description: "Tillåter användare att manipulera objekt vid export."
type: docs
url: /sv/java/com.aspose.cells/iexportobjectlistener/
---
```
public interface IExportObjectListener
```

Tillåter användare att manipulera objekt vid export.

**Example**

Följande exempel skapar en Workbook, öppnar en fil med namnet designer.xls i den och gör de horisontella och vertikala rullningslisterna osynliga för Workbook. Det ersätter sedan två strängvärden med ett heltalsvärde respektive ett strängvärde i kalkylbladet och skickar slutligen den uppdaterade filen till klientens webbläsare.

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
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [exportObject(ExportObjectEvent e)](#exportObject-com.aspose.cells.ExportObjectEvent-) | Exportera ett objekt. |
### exportObject(ExportObjectEvent e) {#exportObject-com.aspose.cells.ExportObjectEvent-}
```
public abstract Object exportObject(ExportObjectEvent e)
```


Exportera ett objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| e | [ExportObjectEvent](../../com.aspose.cells/exportobjectevent) | Händelsen som utlöses när ett objekt behöver exporteras. |

**Returns:**
java.lang.Object – Information om resultatet av export av objektet.

 *  For exporting objects when export workbook to HTML format, the result is URL string to access the saved Image from the html file which contains this exported object.
