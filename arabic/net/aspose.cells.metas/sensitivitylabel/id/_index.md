---
title: "SensitivityLabel.Id"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SensitivityLabel. تحصل وتعيّن معرّف (Id) لعلامة الحساسية"
type: docs
url: /ar/net/aspose.cells.metas/sensitivitylabel/id/
---
## SensitivityLabel.Id property

يحصل على ويضبط معرّف تسمية الحساسية.

```csharp
public string Id { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIdDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // إنشاء نسخة من SensitivityLabel
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // عرض تعيين واسترجاع خاصية Id
                string testId = "CONFIDENTIAL_001";
                label.Id = testId;
                
                // عرض قيمة Id
                Console.WriteLine("Sensitivity Label Id: " + label.Id);
                
                // غيّر قيمة Id لتوضيح أنها قابلة للقراءة والكتابة
                label.Id = "INTERNAL_USE_ONLY";
                Console.WriteLine("Updated Sensitivity Label Id: " + label.Id);
                
                // أظهر أن الخاصية تؤثر على عمليات أخرى
                label.IsEnabled = true;
                Console.WriteLine($"Label {label.Id} is enabled: {label.IsEnabled}");
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


