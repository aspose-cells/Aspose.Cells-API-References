---
title: IExportObjectListener
second_title: Aspose.Cells for Java API Reference
description: Allows users to manipulate objects while exporting.
type: docs
url: /java/com.aspose.cells/iexportobjectlistener/
---
```
public interface IExportObjectListener
```

Allows users to manipulate objects while exporting.

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
## Methods

| Method | Description |
| --- | --- |
| [exportObject(ExportObjectEvent e)](#exportObject-com.aspose.cells.ExportObjectEvent-) | Export one object. |
### exportObject(ExportObjectEvent e) {#exportObject-com.aspose.cells.ExportObjectEvent-}
```
public abstract Object exportObject(ExportObjectEvent e)
```


Export one object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| e | [ExportObjectEvent](../../com.aspose.cells/exportobjectevent) | The event triggered when one object needs to be exported. |

**Returns:**
java.lang.Object - The information about the result of exporting object.

 *  For exporting objects when export workbook to HTML format, the result is URL string to access the saved Image from the html file which contains this exported object.
