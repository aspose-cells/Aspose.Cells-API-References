---
title: "LoadFilter.SheetsInLoadingOrder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadFilter. تحدد مؤشرات الأوراق والترتيب الذي سيتم تحميله. القيمة الافتراضية هي null والتي تعني تحميل جميع الأوراق بالترتيب الافتراضي في ملف القالب. إذا لم تكن null وكان مؤشر بعض الأوراق غير موجود في المصفوفة المرتجعة، فلن يتم تحميل الورقة."
type: docs
url: /ar/net/aspose.cells/loadfilter/sheetsinloadingorder/
---
## LoadFilter.SheetsInLoadingOrder property

يحدد الأوراق (المؤشرات) والترتيب الذي سيتم تحميله. القيمة الافتراضية هي null، مما يعني تحميل جميع الأوراق بالترتيب الافتراضي في ملف القالب. إذا لم تكن null وكان مؤشر بعض الورقة غير موجود في المصفوفة المعادة، فلن يتم تحميل تلك الورقة.

```csharp
public virtual int[] SheetsInLoadingOrder { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LoadFilterPropertySheetsInLoadingOrderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد يحتوي على عدة أوراق
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // إنشاء مرشح تحميل مخصص
            LoadFilter loadFilter = new LoadFilter(LoadDataFilterOptions.All);
            
            // عرض القيمة الافتراضية لـ SheetsInLoadingOrder (null يعني تحميل جميع الأوراق)
            Console.WriteLine("Initial SheetsInLoadingOrder is null: " + (loadFilter.SheetsInLoadingOrder == null));
            
            // إنشاء ملف قالب لتوضيح التحميل بترتيب أوراق مخصص
            workbook.Save("Template.xlsx");
            
            // إنشاء خيارات التحميل باستخدام مرشحنا المخصص
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LoadFilter = loadFilter;
            
            // تحميل المصنف بالإعدادات الافتراضية (جميع الأوراق)
            Workbook loadedWorkbook1 = new Workbook("Template.xlsx", loadOptions);
            Console.WriteLine("Sheets loaded with default filter: " + loadedWorkbook1.Worksheets.Count);
            
            // إنشاء مرشح جديد بترتيب تحميل أوراق محدد
            LoadFilter orderedFilter = new LoadFilter(LoadDataFilterOptions.All)
            {
                // ملاحظة: SheetsInLoadingOrder للقراءة فقط، لذا نحتاج إلى إنشاء مرشح جديد
                // مع الترتيب المطلوب في المُنشئ أو عبر وسائل أخرى
                // هذا يوضح قيود الخاصية كونها للقراءة فقط
            };
            
            // نظرًا لأن SheetsInLoadingOrder للقراءة فقط، سنحتاج إلى إنشاء فئة فرعية من LoadFilter
            // لتوضيح ترتيب تحميل أوراق مخصص
            CustomLoadFilter customFilter = new CustomLoadFilter(new int[] { 2, 0 }); // Load Sheet3 first, then Sheet1
            
            LoadOptions customLoadOptions = new LoadOptions();
            customLoadOptions.LoadFilter = customFilter;
            
            // تحميل المصنف بترتيب أوراق مخصص
            Workbook loadedWorkbook2 = new Workbook("Template.xlsx", customLoadOptions);
            Console.WriteLine("Sheets loaded with custom filter: " + loadedWorkbook2.Worksheets.Count);
            Console.WriteLine("First sheet in custom order: " + loadedWorkbook2.Worksheets[0].Name);
        }
    }

    // تنفيذ LoadFilter مخصص لتوضيح وظيفة SheetsInLoadingOrder
    public class CustomLoadFilter : LoadFilter
    {
        private readonly int[] _sheetsOrder;
        
        public CustomLoadFilter(int[] sheetsOrder) : base(LoadDataFilterOptions.All)
        {
            _sheetsOrder = sheetsOrder;
        }
        
        public override int[] SheetsInLoadingOrder => _sheetsOrder;
    }
}
```

### انظر أيضًا

* class [LoadFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


