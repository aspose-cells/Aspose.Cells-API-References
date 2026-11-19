---
title: "IExportObjectListener"
second_title: "Aspose.Cells for Java API 参考"
description: "允许用户在导出时操作对象。"
type: docs
url: /zh/java/com.aspose.cells/iexportobjectlistener/
---
```
public interface IExportObjectListener
```

允许用户在导出时操作对象。

**Example**

以下示例创建一个 Workbook，打开其中名为 designer.xls 的文件，并使 Workbook 的水平和垂直滚动条不可见。随后在电子表格中分别将两个字符串值替换为整数值和字符串值，最后将更新后的文件发送到客户端浏览器。

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
## 方法

| 方法 | 描述 |
| --- | --- |
| [exportObject(ExportObjectEvent e)](#exportObject-com.aspose.cells.ExportObjectEvent-) | 导出一个对象。 |
### exportObject(ExportObjectEvent e) {#exportObject-com.aspose.cells.ExportObjectEvent-}
```
public abstract Object exportObject(ExportObjectEvent e)
```


导出一个对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| e | [ExportObjectEvent](../../com.aspose.cells/exportobjectevent) | 当需要导出一个对象时触发的事件。 |

**Returns:**
java.lang.Object - 导出对象结果的信息。

 *  For exporting objects when export workbook to HTML format, the result is URL string to access the saved Image from the html file which contains this exported object.
