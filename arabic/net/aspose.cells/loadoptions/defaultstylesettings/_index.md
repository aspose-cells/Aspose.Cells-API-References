---
title: "LoadOptions.DefaultStyleSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تحصل على إعدادات النمط الافتراضية لتهيئة أنماط دفتر العمل"
type: docs
url: /ar/net/aspose.cells/loadoptions/defaultstylesettings/
---
## LoadOptions.DefaultStyleSettings property

يحصل على إعدادات النمط الافتراضية لتهيئة أنماط دفتر العمل

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تعيين خيارات التحميل باستخدام إعدادات النمط الافتراضية
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
            
            // إنشاء ورقة عمل والحصول على الخلايا
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // تعيين القيم لتوضيح النمط الافتراضي
            cells["A1"].PutValue("Default Style Applied");
            cells["A2"].PutValue("Should have bottom alignment");
            
            // إنشاء خلية بنمط مخصص (للمقارنة مع الافتراضي)
            Cell customCell = cells["B1"];
            customCell.PutValue("Custom Style");
            Style customStyle = customCell.GetStyle();
            customStyle.VerticalAlignment = TextAlignmentType.Center;
            customCell.SetStyle(customStyle);
            
            // احفظ المصنف
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
            
            // تحقق من الأنماط
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("B1 Vertical Alignment: " + cells["B1"].GetStyle().VerticalAlignment);
        }
    }
}
```

### انظر أيضًا

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


