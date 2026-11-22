---
title: "SensitivityLabel.IsRemoved"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "SensitivityLabel property. يشير إلى ما إذا تم إزالة تسمية الحساسية"
type: docs
url: /ar/net/aspose.cells.metas/sensitivitylabel/isremoved/
---
## SensitivityLabel.IsRemoved property

يشير إلى ما إذا كانت تسمية الحساسية قد أزيلت.

```csharp
public bool IsRemoved { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyIsRemovedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // أنشئ كائنًا لتسمية الحساسية عبر الانعكاس
                // لأن إنشاء مباشر غير متاح
                Type labelType = typeof(SensitivityLabel);
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(labelType);
                
                // حدد الخصائص المطلوبة
                label.Id = "SENSITIVE_DATA";
                label.IsEnabled = true;
                label.IsRemoved = false;
                
                // اعرض القيمة الأولية لـ IsRemoved
                Console.WriteLine("Initial IsRemoved value: " + label.IsRemoved);
                
                // أظهر ضبط خاصية IsRemoved (لأنها قابلة للقراءة والكتابة)
                label.IsRemoved = true;
                Console.WriteLine("After setting IsRemoved: " + label.IsRemoved);
                
                // بدّل القيمة مرة أخرى لتظهر أنه يمكن تغييرها
                label.IsRemoved = false;
                Console.WriteLine("Final IsRemoved value: " + label.IsRemoved);
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


