---
title: "IExportObjectListener"
second_title: "Справочник API Aspose.Cells for Java"
description: "Позволяет пользователям манипулировать объектами во время экспорта."
type: docs
url: /ru/java/com.aspose.cells/iexportobjectlistener/
---
```
public interface IExportObjectListener
```

Позволяет пользователям манипулировать объектами во время экспорта.

**Example**

В следующем примере создаётся Workbook, открывается файл с именем designer.xls и делаются горизонтальная и вертикальная полосы прокрутки невидимыми для Workbook. Затем в таблице заменяются два строковых значения на значение типа Integer и строковое значение соответственно, и в конце обновлённый файл отправляется в браузер клиента.

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
## Методы

| Метод | Описание |
| --- | --- |
| [exportObject(ExportObjectEvent e)](#exportObject-com.aspose.cells.ExportObjectEvent-) | Экспортировать один объект. |
### exportObject(ExportObjectEvent e) {#exportObject-com.aspose.cells.ExportObjectEvent-}
```
public abstract Object exportObject(ExportObjectEvent e)
```


Экспортировать один объект.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| e | [ExportObjectEvent](../../com.aspose.cells/exportobjectevent) | Событие, вызываемое, когда необходимо экспортировать один объект. |

**Returns:**
java.lang.Object — Информация о результате экспорта объекта.

 *  For exporting objects when export workbook to HTML format, the result is URL string to access the saved Image from the html file which contains this exported object.
