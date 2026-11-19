---
title: "IExportObjectListener"
second_title: "Aspose.Cells for Java API Reference"
description: "يسمح للمستخدمين بالتلاعب بالكائنات أثناء التصدير."
type: docs
url: /ar/java/com.aspose.cells/iexportobjectlistener/
---
```
public interface IExportObjectListener
```

يسمح للمستخدمين بالتلاعب بالكائنات أثناء التصدير.

**Example**

المثال التالي ينشئ مصنفًا، يفتح ملفًا باسم designer.xls فيه ويجعل أشرطة التمرير الأفقية والعمودية غير مرئية للمصنف. ثم يستبدل قيمتين نصيتين بقيمة عددية وقيمة نصية على التوالي داخل جدول البيانات وأخيرًا يرسل الملف المحدث إلى متصفح العميل.

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
## الطرق

| طريقة | الوصف |
| --- | --- |
| [exportObject(ExportObjectEvent e)](#exportObject-com.aspose.cells.ExportObjectEvent-) | تصدير كائن واحد. |
### exportObject(ExportObjectEvent e) {#exportObject-com.aspose.cells.ExportObjectEvent-}
```
public abstract Object exportObject(ExportObjectEvent e)
```


تصدير كائن واحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| e | [ExportObjectEvent](../../com.aspose.cells/exportobjectevent) | الحدث الذي يتم تشغيله عندما يحتاج كائن واحد إلى التصدير. |

**Returns:**
java.lang.Object - المعلومات حول نتيجة تصدير الكائن.

 *  For exporting objects when export workbook to HTML format, the result is URL string to access the saved Image from the html file which contains this exported object.
