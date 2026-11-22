---
title: "LoadOptions.MemorySetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تحصل أو تعين وضع الذاكرة لدفتر العمل المحمّل"
type: docs
url: /ar/net/aspose.cells/loadoptions/memorysetting/
---
## LoadOptions.MemorySetting property

يحصل على أو يضبط وضع الذاكرة لدفتر العمل المحمَّل.

```csharp
public MemorySetting MemorySetting { get; set; }
```

### ملاحظات

لمزيد من التفاصيل حول وضع الذاكرة، يرجى الاطلاع على [`MemorySetting`](../../cells/memorysetting/).

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyMemorySettingDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل مع تعيين تفضيل الذاكرة
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
            loadOptions.MemorySetting = MemorySetting.MemoryPreference;

            // تحميل دفتر العمل بإعدادات تحسين الذاكرة
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // الوصول إلى ورقة العمل وإضافة بعض بيانات العينة
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Memory Setting Demo");
            worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
            
            // احفظ المصنف
            workbook.Save("MemorySettingDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with MemoryPreference setting.");
        }
    }
}
```

### انظر أيضًا

* enum [MemorySetting](../../memorysetting/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


