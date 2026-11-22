---
title: "LoadFilter.LoadFilter"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ LoadFilter. ينشئ LoadFilter واحد مع خيارات الفلتر الافتراضية LoadDataFilterOptions.All"
type: docs
url: /ar/net/aspose.cells/loadfilter/loadfilter/
---
## LoadFilter() {#constructor}

ينشئ LoadFilter واحد مع خيارات الفلتر الافتراضية LoadDataFilterOptions.All.

```csharp
public LoadFilter()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadFilterMethodCtorDemo
    {
        public static void Run()
        {
            // إنشاء LoadFilter جديد باستخدام المنشئ الافتراضي
            LoadFilter filter = new LoadFilter();
            
            // إنشاء خيارات التحميل وتعيين الفلتر
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = filter;
            
            // تحميل دفتر العمل باستخدام الفلتر
            Workbook workbook = new Workbook("sample.xlsx", loadOptions);
            
            // عرض الاستخدام عن طريق عد أوراق العمل
            Console.WriteLine("Number of worksheets loaded: " + workbook.Worksheets.Count);
            
            // إظهار بيانات الخلايا المفلترة (جميع الخلايا يتم تحميلها افتراضيًا)
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                Console.WriteLine($"Worksheet '{sheet.Name}' has {sheet.Cells.Count} cells");
            }
        }
    }
}
```

### انظر أيضًا

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## LoadFilter(LoadDataFilterOptions) {#constructor_1}

ينشئ LoadFilter واحد مع خيارات الفلتر المحددة.

```csharp
public LoadFilter(LoadDataFilterOptions opts)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| opts | LoadDataFilterOptions | خيارات الفلتر الافتراضية |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterMethodCtorWithLoadDataFilterOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير البيانات لمعلمات الطريقة (LoadDataFilterOptions)
            LoadDataFilterOptions filterOptions = LoadDataFilterOptions.CellData | LoadDataFilterOptions.Chart;

            try
            {
                // استدعاء طريقة #ctor بالأنواع المحددة للمعاملات
                LoadFilter loadFilter = new LoadFilter(filterOptions);

                // معالجة أو عرض النتيجة
                Console.WriteLine("LoadFilter created successfully with LoadDataFilterOptions: " + filterOptions);

                // إظهار تأثير استدعاء الطريقة
                Console.WriteLine("LoadDataFilterOptions set to: " + loadFilter.LoadDataFilterOptions);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error creating LoadFilter: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("LoadFilterCtorWithLoadDataFilterOptionsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [LoadDataFilterOptions](../../loaddatafilteroptions/)
* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


