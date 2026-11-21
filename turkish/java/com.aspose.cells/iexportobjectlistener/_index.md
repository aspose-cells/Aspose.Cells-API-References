---
title: "IExportObjectListener"
second_title: "Aspose.Cells for Java API Referansı"
description: "Kullanıcıların dışa aktarım sırasında nesneleri manipüle etmelerine izin verir."
type: docs
url: /tr/java/com.aspose.cells/iexportobjectlistener/
---
```
public interface IExportObjectListener
```

Kullanıcıların dışa aktarım sırasında nesneleri manipüle etmelerine izin verir.

**Example**

Aşağıdaki örnek bir Workbook oluşturur, içinde designer.xls adlı bir dosya açar ve Workbook için yatay ve dikey kaydırma çubuklarını görünmez yapar. Ardından elektronik tablo içinde iki dize değerini sırasıyla bir Integer değeri ve bir dize değeriyle değiştirir ve sonunda güncellenen dosyayı istemci tarayıcısına gönderir.

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
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [exportObject(ExportObjectEvent e)](#exportObject-com.aspose.cells.ExportObjectEvent-) | Bir nesneyi dışa aktar. |
### exportObject(ExportObjectEvent e) {#exportObject-com.aspose.cells.ExportObjectEvent-}
```
public abstract Object exportObject(ExportObjectEvent e)
```


Bir nesneyi dışa aktar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| e | [ExportObjectEvent](../../com.aspose.cells/exportobjectevent) | Bir nesnenin dışa aktarılması gerektiğinde tetiklenen olay. |

**Returns:**
java.lang.Object - Nesneyi dışa aktarma sonucuyla ilgili bilgi.

 *  For exporting objects when export workbook to HTML format, the result is URL string to access the saved Image from the html file which contains this exported object.
