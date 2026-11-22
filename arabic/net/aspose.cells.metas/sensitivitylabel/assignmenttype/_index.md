---
title: "SensitivityLabel.AssignmentType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "SensitivityLabel property. يحصل على طريقة تعيين تسمية الحساسية ويضبطها"
type: docs
url: /ar/net/aspose.cells.metas/sensitivitylabel/assignmenttype/
---
## SensitivityLabel.AssignmentType property

يحصل على ويضبط طريقة التعيين لتسمية الحساسية.

```csharp
public SensitivityLabelAssignmentType AssignmentType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyAssignmentTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            try
            {
                // إنشاء نسخة من SensitivityLabel
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // تعيين الخصائص الأساسية
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                
                // أظهر الحصول على القيمة الأولية لـ AssignmentType
                Console.WriteLine("Initial AssignmentType: " + label.AssignmentType);
                
                // قم بتعيين AssignmentType إلى Privileged وعرض التغيير
                label.AssignmentType = SensitivityLabelAssignmentType.Privileged;
                Console.WriteLine("After setting Privileged: " + label.AssignmentType);
                
                // غيّر مرة أخرى إلى Standard لتوضيح أنه قابل للقراءة والكتابة
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                Console.WriteLine("After setting Standard: " + label.AssignmentType);
                
                // احفظ المصنف
                workbook.Save("AssignmentTypeDemo.xlsx");
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

* enum [SensitivityLabelAssignmentType](../../sensitivitylabelassignmenttype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


