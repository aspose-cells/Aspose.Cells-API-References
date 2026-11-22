---
title: "LoadFilter.StartSheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة LoadFilter. تُعد خيارات الفلتر قبل تحميل ورقة العمل المحددة. يمكن لتطبيق المستخدم لـ LoadFilter تعديل LoadDataFilterOptions هنا لتحديد كيفية تحميل البيانات لهذه الورقة."
type: docs
url: /ar/net/aspose.cells/loadfilter/startsheet/
---
## LoadFilter.StartSheet method

يجهز خيارات الفلتر قبل تحميل ورقة العمل المحددة. يمكن لتطبيق المستخدم لـ LoadFilter تغيير LoadDataFilterOptions هنا لتحديد كيفية تحميل البيانات لهذه الورقة.

```csharp
public virtual void StartSheet(Worksheet sheet)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ورقة | ورقة العمل | ورقة العمل التي سيتم تحميلها. هناك عدد قليل فقط من الخصائص التي يمكن استخدامها لكائن ورقة العمل المحددة هنا لأن معظم البيانات والخصائص لم يتم تحميلها. الخصائص المتاحة هي: Name, Index, VisibilityType |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodStartSheetWithWorksheetDemo
    {
        // إنشاء فئة فلتر تحميل مخصصة تمتد من LoadFilter
        class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                Console.WriteLine($"Processing sheet: {sheet.Name}");
                // يمكنك إضافة منطق مخصص هنا للتعامل مع أوراق محددة
            }
        }

        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "TestSheet";

            // إنشاء مثال من فلتر التحميل المخصص الخاص بنا
            CustomLoadFilter loadFilter = new CustomLoadFilter();

            try
            {
                // استدعاء طريقة StartSheet مع معامل ورقة العمل
                loadFilter.StartSheet(worksheet);
                
                Console.WriteLine("StartSheet method executed successfully");
                
                // إضافة بعض البيانات لإظهار أن الورقة قابلة للوصول
                worksheet.Cells["A1"].PutValue("StartSheet Demo");
                worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("LoadFilterStartSheetDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../worksheet/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


