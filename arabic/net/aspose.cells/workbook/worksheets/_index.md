---
title: "Workbook.Worksheets"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. يحصل على مجموعة WorksheetCollection في جدول البيانات"
type: docs
url: /ar/net/aspose.cells/workbook/worksheets/
---
## Workbook.Worksheets property

يحصل على مجموعة [`WorksheetCollection`](../../worksheetcollection/) في جدول البيانات.

```csharp
public WorksheetCollection Worksheets { get; }
```

### قيمة الإرجاع

[`WorksheetCollection`](../../worksheetcollection/) collection

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyWorksheetsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // إضافة ورقة عمل جديدة
            workbook.Worksheets.Add("SecondSheet");
            
            // الوصول إلى ورقة العمل الثانية وإضافة البيانات
            Worksheet secondSheet = workbook.Worksheets[1];
            secondSheet.Cells["A1"].PutValue("Product");
            secondSheet.Cells["B1"].PutValue("Price");
            secondSheet.Cells["A2"].PutValue("Laptop");
            secondSheet.Cells["B2"].PutValue(999.99);
            
            // احفظ المصنف
            workbook.Save("WorkbookWorksheetsDemo.xlsx");
            
            // إخراج عدد أوراق العمل
            Console.WriteLine($"Number of worksheets: {workbook.Worksheets.Count}");
        }
    }
}
```

### انظر أيضًا

* class [WorksheetCollection](../../worksheetcollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


