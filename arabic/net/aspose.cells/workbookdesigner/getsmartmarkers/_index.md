---
title: "WorkbookDesigner.GetSmartMarkers"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorkbookDesigner. تُرجع مجموعة من العلامات الذكية في جدول بيانات"
type: docs
url: /ar/net/aspose.cells/workbookdesigner/getsmartmarkers/
---
## WorkbookDesigner.GetSmartMarkers method

يرجع مجموعة من العلامات الذكية في جدول بيانات.

```csharp
public string[] GetSmartMarkers()
```

### قيمة الإرجاع

مجموعة من العلامات الذكية

### ملاحظات

يتم إنشاء مصفوفة سلاسل نصية في كل استدعاء. يتم فرز المصفوفة وإزالة القيم المكررة.

### أمثلة

```csharp
using System;
using System.Data;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodGetSmartMarkersDemo
    {
        public static void Run()
        {
            // إنشاء ملف قالب تجريبي في الذاكرة
            Workbook templateWorkbook = new Workbook();
            Cells cells = templateWorkbook.Worksheets[0].Cells;
            
            // إضافة العلامات الذكية إلى القالب
            cells["A1"].PutValue("&=COLORS_TIMES.COLORS");
            cells["B1"].PutValue("&=COLORS_TIMES.TIMES");
            
            // حفظ القالب إلى تدفق الذاكرة
            MemoryStream templateStream = new MemoryStream();
            templateWorkbook.Save(templateStream, SaveFormat.Xlsx);
            
            // تهيئة WorkbookDesigner باستخدام القالب
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = new Workbook(templateStream);
            
            // الحصول على العلامات الذكية وعرضها
            string[] smartMarkers = designer.GetSmartMarkers();
            Console.WriteLine("Found smart markers:");
            foreach (string marker in smartMarkers)
            {
                Console.WriteLine(marker);
            }
            
            // تحضير مصدر البيانات
            DataTable data = new DataTable("COLORS_TIMES");
            data.Columns.Add("COLORS", typeof(string));
            data.Columns.Add("TIMES", typeof(DateTime));
            data.Rows.Add("red", DateTime.Now.AddDays(-1));
            data.Rows.Add("yellow", DateTime.Now);
            data.Rows.Add("green", DateTime.Now.AddDays(1));
            
            // تعيين مصدر البيانات ومعالجته
            designer.SetDataSource(data);
            designer.Process();
            
            // حفظ النتيجة
            designer.Workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


