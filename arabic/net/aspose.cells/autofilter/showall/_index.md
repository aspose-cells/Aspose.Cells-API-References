---
title: "AutoFilter.ShowAll"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة AutoFilter. إلغاء إخفاء جميع الصفوف"
type: docs
url: /ar/net/aspose.cells/autofilter/showall/
---
## AutoFilter.ShowAll method

إظهار جميع الصفوف.

```csharp
public void ShowAll()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFilterMethodShowAllDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["A5"].PutValue("Grape");
            
            // تطبيق الفلتر التلقائي
            worksheet.AutoFilter.Range = "A1:A5";
            
            // تصفية لإظهار "Apple" فقط
            worksheet.AutoFilter.Filter(0, "Apple");
            
            // إظهار جميع البيانات مرة أخرى
            worksheet.AutoFilter.ShowAll();
            
            // احفظ المصنف
            workbook.Save("ShowAllDemoOutput.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


