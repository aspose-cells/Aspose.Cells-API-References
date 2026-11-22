---
title: "الواجهة IExportObjectListener"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الواجهة Aspose.Cells.IExportObjectListener. تسمح للمستخدمين بالتلاعب بالكائنات أثناء التصدير"
type: docs
url: /ar/net/aspose.cells/iexportobjectlistener/
---
## IExportObjectListener interface

يسمح للمستخدمين بالتلاعب بالكائنات أثناء التصدير.

```csharp
public interface IExportObjectListener
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [ExportObject](../../aspose.cells/iexportobjectlistener/exportobject/)(ExportObjectEvent) | صدّر كائنًا واحدًا. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CellsClassIExportObjectListenerDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف صورة نموذجية إلى ورقة العمل
            int pictureIndex = worksheet.Pictures.Add(0, 0, "example.png");
            Picture picture = worksheet.Pictures[pictureIndex];
            
            // تنفيذ مستمع تصدير مخصص
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportObjectListener = new CustomExportObjectListener();
            
            // احفظ إلى HTML باستخدام مستمع مخصص
            workbook.Save("output.html", saveOptions);
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;
        
        public object ExportObject(ExportObjectEvent e)
        {
            object source = e.GetSource();
            if (source is Shape)
            {
                Shape shape = (Shape)source;
                if (shape.MsoDrawingType == MsoDrawingType.Picture)
                {
                    string url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
                    imgIdx++;
                    return url;
                }
            }
            return null;
        }
        
        private string SaveImage(byte[] data, int imgIdx, ImageType format)
        {
            // في تنفيذ حقيقي، ستقوم بحفظ الصورة على القرص هنا
            // لأغراض العرض، نعيد فقط مسارًا تجريبيًا
            return $"images/image_{imgIdx}.png";
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


