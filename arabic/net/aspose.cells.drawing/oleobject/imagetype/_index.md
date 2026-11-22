---
title: "OleObject.ImageType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObject. تحصل على تنسيق الصورة لكائن ole"
type: docs
url: /ar/net/aspose.cells.drawing/oleobject/imagetype/
---
## OleObject.ImageType property

يحصل على تنسيق الصورة لكائن OLE.

```csharp
public ImageType ImageType { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectPropertyImageTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة كائن OLE إلى ورقة العمل
            byte[] fileData = File.ReadAllBytes(@"C:\example.xlsx");
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            // اعرض نوع الصورة الحالي لكائن OLE
            Console.WriteLine("Current ImageType value: " + oleObject.ImageType);

            // وضح كيفية استخدام خاصية ImageType
            if (oleObject.ImageType == ImageType.Unknown)
            {
                Console.WriteLine("The OLE object's image format is not recognized.");
            }
            else if (oleObject.ImageType == ImageType.Emf)
            {
                Console.WriteLine("The OLE object uses EMF image format.");
            }
            else if (oleObject.ImageType == ImageType.Png)
            {
                Console.WriteLine("The OLE object uses PNG image format.");
            }

            // احفظ المصنف
            workbook.Save("OleObjectImageTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ImageType](../../imagetype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


