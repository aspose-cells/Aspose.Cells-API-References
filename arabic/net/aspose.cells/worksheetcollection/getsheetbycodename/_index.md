---
title: "WorksheetCollection.GetSheetByCodeName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorksheetCollection. تحصل على ورقة العمل بواسطة اسم الكود"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/getsheetbycodename/
---
## WorksheetCollection.GetSheetByCodeName method

يحصل على ورقة العمل بالاسم الرمزي.

```csharp
public Worksheet GetSheetByCodeName(string codeName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| codeName | String | اسم كود ورقة العمل. |

### قيمة الإرجاع

العنصر ذو اسم الكود المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetSheetByCodeNameWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة أوراق عمل وتعيين أسماء الكود الخاصة بها
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            sheet1.CodeName = "MainSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.CodeName = "DataSheet";

            // الحصول على ورقة العمل بواسطة اسم الكود
            Worksheet mainSheet = workbook.Worksheets.GetSheetByCodeName("MainSheet");
            Worksheet dataSheet = workbook.Worksheets.GetSheetByCodeName("DataSheet");

            // إظهار الاستخدام عن طريق الكتابة في الخلايا
            mainSheet.Cells["A1"].PutValue("This is Main Sheet");
            dataSheet.Cells["A1"].PutValue("This is Data Sheet");

            // احفظ المصنف
            workbook.Save("GetSheetByCodeNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


