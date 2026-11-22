---
title: "الفئة LoadFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.LoadFilter. تمثل الفلتر الذي يوفر خيارات لتحميل البيانات عند تحميل المصنف من القالب"
type: docs
url: /ar/net/aspose.cells/loadfilter/
---
## LoadFilter class

يمثل الفلتر الذي يوفر خيارات تحميل البيانات عند تحميل المصنف من القالب.

```csharp
public class LoadFilter
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LoadFilter](loadfilter/#constructor)() | ينشئ LoadFilter واحد مع خيارات الفلتر الافتراضية LoadDataFilterOptions.All. |
| [LoadFilter](loadfilter/#constructor_1)(LoadDataFilterOptions) | ينشئ LoadFilter واحد مع خيارات الفلتر المحددة. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [LoadDataFilterOptions](../../aspose.cells/loadfilter/loaddatafilteroptions/) { get; set; } | خيارات الفلتر لتحديد البيانات التي يجب تحميلها. |
| virtual [SheetsInLoadingOrder](../../aspose.cells/loadfilter/sheetsinloadingorder/) { get; } | يحدد الأوراق (المؤشرات) والترتيب الذي سيتم تحميله. القيمة الافتراضية هي null، مما يعني تحميل جميع الأوراق بالترتيب الافتراضي في ملف القالب. إذا لم تكن null وكان مؤشر بعض الورقة غير موجود في المصفوفة المعادة، فلن يتم تحميل تلك الورقة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [StartSheet](../../aspose.cells/loadfilter/startsheet/)(Worksheet) | يجهز خيارات الفلتر قبل تحميل ورقة العمل المحددة. يمكن لتطبيق المستخدم لـ LoadFilter تغيير LoadDataFilterOptions هنا لتحديد كيفية تحميل البيانات لهذه الورقة. |

### ملاحظات

يمكن للمستخدم تحديد خيارات الفلتر أو تنفيذ LoadFilter الخاص به لتحديد طريقة تحميل البيانات.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterDemo
    {
        public static void LoadFilterExample()
        {
            // إنشاء LoadOptions وتعيين LoadFilter
            LoadOptions opts = new LoadOptions();
            opts.LoadFilter = new CustomLoadFilter();

            // تحميل المصنف باستخدام LoadOptions المحددة
            Workbook wb = new Workbook("LoadFilterExample_original.xlsx", opts);

            // احفظ المصنف لرؤية تأثير LoadFilter
            wb.Save("LoadFilterExample.xlsx");
        }

        // تنفيذ LoadFilter مخصص
        public class CustomLoadFilter : LoadFilter
        {
            public override void StartSheet(Worksheet sheet)
            {
                if (sheet.Name == "Sheet1")
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.All;
                }
                else
                {
                    LoadDataFilterOptions = LoadDataFilterOptions.Structure;
                }
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


