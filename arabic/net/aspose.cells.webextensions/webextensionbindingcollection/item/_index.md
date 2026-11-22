---
title: "WebExtensionBindingCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WebExtensionBindingCollection. تحصل على علاقة ربط امتداد الويب وفق الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.webextensions/webextensionbindingcollection/item/
---
## WebExtensionBindingCollection indexer

يحصل على علاقة ربط امتداد الويب حسب الفهرس المحدد.

```csharp
public WebExtensionBinding this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### قيمة الإرجاع

علاقة ربط امتداد الويب

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionBindingCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مجموعة ربط امتداد الويب
            WebExtensionBindingCollection bindingCollection = new WebExtensionBindingCollection();

            // إضافة ربط جديد إلى المجموعة
            int index = bindingCollection.Add();

            // الوصول إلى الربط باستخدام خاصية Item (للقراءة فقط)
            WebExtensionBinding binding = bindingCollection[index];

            // ضبط الخصائص على الربط
            binding.Id = "binding1";
            binding.Type = "Text";
            binding.Appref = "Sheet1!A1";

            // عرض تفاصيل الربط
            Console.WriteLine("Binding ID: " + binding.Id);
            Console.WriteLine("Binding Type: " + binding.Type);
            Console.WriteLine("Binding AppRef: " + binding.Appref);

            // تعديل الربط عبر المجموعة
            bindingCollection[index].Id = "modifiedBinding";
            Console.WriteLine("Modified Binding ID: " + bindingCollection[index].Id);

            // احفظ المصنف
            workbook.Save("WebExtensionBindingDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WebExtensionBinding](../../webextensionbinding/)
* class [WebExtensionBindingCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


