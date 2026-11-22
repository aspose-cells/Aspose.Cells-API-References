---
title: "فئة ExportObjectEvent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.ExportObjectEvent. الحدث الذي يتم تشغيله عند تصدير كائن مثل Picture"
type: docs
url: /ar/net/aspose.cells/exportobjectevent/
---
## ExportObjectEvent class

الحدث الذي يتم تشغيله عند تصدير كائن، مثل Picture.

```csharp
public class ExportObjectEvent
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetSource](../../aspose.cells/exportobjectevent/getsource/)() | يحصل على الكائن المراد تصديره. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ExportObjectEventDemo
    {
        public static void ExportObjectEventExample()
        {
            // تنفيذ مخصص لـ IExportObjectListener
            // احفظ ملف HTML مع مستمع مخصص
            Workbook workbook = new Workbook(); // Build your workbook here
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportObjectListener = new CustomExportObjectListener()
            };
            using (Stream stream = new FileStream("ExportObjectEventExample.html", FileMode.Create))
            {
                workbook.Save(stream, saveOptions); // Save the workbook to stream
            }
        }
    }

    class CustomExportObjectListener : IExportObjectListener
    {
        private int imgIdx = 0;

        public object ExportObject(ExportObjectEvent e)
        {
            object source = e.GetSource();
            if (source is Shape shape)
            {
                string url = null;
                switch (shape.MsoDrawingType)
                {
                    case MsoDrawingType.Picture:
                        url = SaveImage(((Picture)shape).Data, imgIdx, ((Picture)shape).ImageType);
                        break;
                }
                if (url != null)
                {
                    imgIdx++;
                }
                return url;
            }
            return null;
        }

        private string SaveImage(byte[] data, int imgIdx, ImageType format)
        {
            // هنا احفظ الصورة في أي موقع، ثم أعد عنوان URL (نسبي أو مطلق) الذي يمكن لملف HTML المُولد الحصول على الصورة منه
            return $"temp{imgIdx}/temp{imgIdx}.png";
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


