---
title: IExportObjectListener
second_title: Aspose.Cells for .NET API 参考
description: 允许用户在导出时操作对象
type: docs
weight: 3790
url: /zh/net/aspose.cells/iexportobjectlistener/
---
## IExportObjectListener interface

允许用户在导出时操作对象。

```csharp
public interface IExportObjectListener
```

## 方法

| 姓名 | 描述 |
| --- | --- |
| [ExportObject](../../aspose.cells/iexportobjectlistener/exportobject)(ExportObjectEvent) | 导出一个对象。 |

### 例子

下面的示例创建一个工作簿，在其中打开一个名为 Designer.xls 的文件，并使水平和工作簿不可见的垂直滚动条。然后，它在电子表格中分别用整数值和字符串值替换两个字符串值，最后将更新后的文件发送到客户端浏览器。

```csharp
[C#]
     //IExportObjectListener

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
            //这里将图片保存到任意位置，然后返回生成的html可以获取到image

            return "temp1/temp2.png";
        }
     }
     
      //用自定义listener

        HtmlSaveOptions saveOptions = new HtmlSaveOptions();
        saveOptions.ExportObjectListener = new CustomExportObjectListener();
        Stream stream = File.Create(outfn);
        book.Save(stream, saveOptions);
        stream.Flush();
        stream.Close();

```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->