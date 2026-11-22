---
title: "SensitivityLabel.IsEnabled"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "SensitivityLabel property. يشير إلى ما إذا كانت تسمية الحساسية مفعلة"
type: docs
url: /ar/net/aspose.cells.metas/sensitivitylabel/isenabled/
---
## SensitivityLabel.IsEnabled property

يشير إلى ما إذا كانت تسمية الحساسية مفعلة

```csharp
public bool IsEnabled { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIsEnabledDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // إنشاء نسخة من SensitivityLabel
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // حدد الخصائص الأولية
                label.Id = "CONFIDENTIAL_001";
                
                // أظهر الحصول على القيمة الأولية لـ IsEnabled
                Console.WriteLine("Initial IsEnabled value: " + label.IsEnabled);
                
                // عيّن IsEnabled إلى true وعرض التغيير
                label.IsEnabled = true;
                Console.WriteLine("After enabling: " + label.IsEnabled);
                
                // بدّل القيمة لتظهر أنها قابلة للقراءة والكتابة
                label.IsEnabled = false;
                Console.WriteLine("After disabling: " + label.IsEnabled);
                
                // احفظ المصنف
                workbook.Save("IsEnabledDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


