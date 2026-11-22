---
title: "DocxSaveOptions.SaveElementType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DocxSaveOptions. تشير إلى العناصر التي يجب حفظها"
type: docs
url: /ar/net/aspose.cells/docxsaveoptions/saveelementtype/
---
## DocxSaveOptions.SaveElementType property

يشير إلى العناصر التي يجب حفظها.

```csharp
public SaveElementType SaveElementType { get; set; }
```

### أمثلة

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class DocxSaveOptionsPropertySaveElementTypeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد وإضافة بعض البيانات النموذجية
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo Data");

            try
            {
                // تهيئة DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // ملاحظة: خاصية SaveElementType غير موجودة في فئة DocxSaveOptions
                // استنادًا إلى انعكاس API المقدم. إذا كانت موجودة، كنت ستقرأها هكذا:
                // var elementType = saveOptions.SaveElementType;
                // Console.WriteLine("SaveElementType: " + elementType);

                // توضيح قراءة خاصية موجودة: SaveAsEditableShaps
                Console.WriteLine("SaveAsEditableShaps (default): " + saveOptions.SaveAsEditableShaps);

                // تعيين الخاصية إلى true وعرض القيمة الجديدة
                saveOptions.SaveAsEditableShaps = true;
                Console.WriteLine("SaveAsEditableShaps (after set): " + saveOptions.SaveAsEditableShaps);

                // حفظ المصنف كملف DOCX باستخدام الخيارات المكوّنة
                workbook.Save("SaveElementTypeDemo.docx", saveOptions);
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* enum [SaveElementType](../../../aspose.cells.saving/saveelementtype/)
* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


