---
title: "Workbook.RemovePersonalInformation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Workbook. تزيل المعلومات الشخصية"
type: docs
url: /ar/net/aspose.cells/workbook/removepersonalinformation/
---
## Workbook.RemovePersonalInformation method

يزيل المعلومات الشخصية.

```csharp
public void RemovePersonalInformation()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemovePersonalInformationDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // أضف تعليقًا بمعلومات المؤلف
            int commentIndex = sheet.Comments.Add("A1");
            sheet.Comments[commentIndex].Note = "Sample comment";
            sheet.Comments[commentIndex].Author = "Test Author";
            
            // اعرض معلومات المؤلف الأصلية
            Console.WriteLine("Before removal - Comment Author: " + sheet.Comments[commentIndex].Author);
            
            // إزالة المعلومات الشخصية
            wb.RemovePersonalInformation();
            
            // احفظ المصنف
            wb.Save("output.xlsx", SaveFormat.Xlsx);
            
            // أعد التحميل للتحقق من الإزالة
            Workbook wb2 = new Workbook("output.xlsx");
            Console.WriteLine("After removal - Comment Author: " + wb2.Worksheets[0].Comments[commentIndex].Author);
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


