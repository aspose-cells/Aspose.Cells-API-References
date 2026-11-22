---
title: "OleObjectCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OleObjectCollection. تحصل على عنصر OleObject عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.drawing/oleobjectcollection/item/
---
## OleObjectCollection indexer

يحصل على عنصر [`OleObject`](../../oleobject/) عند الفهرس المحدد.

```csharp
public OleObject this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة بيانات صورة عينة
            byte[] binaryImg = File.ReadAllBytes("image1.png");
            
            // إضافة كائن OLE إلى ورقة العمل الأولى
            int idxOle = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, binaryImg);
            
            // الوصول إلى كائن OLE باستخدام خاصية Item
            OleObject objOle = workbook.Worksheets[0].OleObjects[idxOle];
            
            // تعيين خصائص الكائن المضمّن
            byte[] binaryXlsx = File.ReadAllBytes("example.xlsx");
            objOle.SetEmbeddedObject(false, binaryXlsx, "SampleFile.xlsx", true, "Excel.Sheet", false);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
            
            // تحقق من الملف المحفوظ
            Workbook savedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("OLE Object Source: " + savedWorkbook.Worksheets[0].OleObjects[0].ObjectSourceFullName);
        }
    }
}
```

### انظر أيضًا

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


