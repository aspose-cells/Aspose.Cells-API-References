---
title: "ListObject.RemoveAutoFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ListObject. تزيل الفلتر التلقائي المطبق على هذا الجدول"
type: docs
url: /ar/net/aspose.cells.tables/listobject/removeautofilter/
---
## ListObject.RemoveAutoFilter method

يزيل التصفية التلقائية المطبقة على هذا الجدول.

```csharp
public void RemoveAutoFilter()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodRemoveAutoFilterDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // ملء بيانات عينة (مع صف الرأس)
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Name");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue("Alice");
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue("Bob");
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B4"].PutValue("Charlie");

            try
            {
                // إضافة كائن ListObject (جدول) يتضمن مرشحًا تلقائيًا بشكل افتراضي
                int listIndex = sheet.ListObjects.Add("A1", "B4", true);
                ListObject listObj = sheet.ListObjects[listIndex];

                // اختياري: تطبيق مرشح لإظهار أن هناك مرشحًا
                listObj.Filter();

                // إزالة المرشح التلقائي من كائن ListObject
                listObj.RemoveAutoFilter();

                Console.WriteLine("RemoveAutoFilter called successfully.");
                
                // احفظ المصنف للتحقق من التغييرات
                workbook.Save("RemoveAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during RemoveAutoFilter operation: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


