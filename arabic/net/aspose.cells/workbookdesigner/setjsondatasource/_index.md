---
title: "WorkbookDesigner.SetJsonDataSource"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorkbookDesigner. تعيين قيمة سلسلة json كمصدر بيانات للعلامات الذكية"
type: docs
url: /ar/net/aspose.cells/workbookdesigner/setjsondatasource/
---
## WorkbookDesigner.SetJsonDataSource method

تعيين قيمة سلسلة JSON كمصدر بيانات للعلامات الذكية.

```csharp
public void SetJsonDataSource(string name, string json)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الجدول. إذا كانت قيمة JSON تمثل كائنًا، قد تكون null. |
| json | String | قيمة سلسلة Json. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodSetJsonDataSourceWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة علامة تجريبية في الخلية A1
            worksheet.Cells["A1"].PutValue("&=$DataSource.Name");
            
            // إنشاء مصمم دفتر عمل
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            
            // عينة بيانات JSON
            string jsonData = "{\"Name\":\"John Doe\",\"Age\":30,\"City\":\"New York\"}";
            
            // تعيين مصدر بيانات JSON
            designer.SetJsonDataSource("DataSource", jsonData);
            
            // معالجة العلامات
            designer.Process();
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


