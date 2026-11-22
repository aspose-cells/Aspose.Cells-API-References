---
title: "فئة SensitivityLabel"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.Metas.SensitivityLabel. تمثل تسمية الحساسية"
type: docs
url: /ar/net/aspose.cells.metas/sensitivitylabel/
---
## SensitivityLabel class

يمثل تصنيف الحساسية.

```csharp
public class SensitivityLabel
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AssignmentType](../../aspose.cells.metas/sensitivitylabel/assignmenttype/) { get; set; } | يحصل على ويضبط طريقة التعيين لتسمية الحساسية. |
| [ContentMarkType](../../aspose.cells.metas/sensitivitylabel/contentmarktype/) { get; set; } | يحصل على ويضبط أنواع تمييز المحتوى التي يجب تطبيقها على ملف. |
| [Id](../../aspose.cells.metas/sensitivitylabel/id/) { get; set; } | يحصل على ويضبط معرّف تسمية الحساسية. |
| [IsEnabled](../../aspose.cells.metas/sensitivitylabel/isenabled/) { get; set; } | يشير إلى ما إذا كانت تسمية الحساسية مفعلة |
| [IsRemoved](../../aspose.cells.metas/sensitivitylabel/isremoved/) { get; set; } | يشير إلى ما إذا كانت تسمية الحساسية قد أزيلت. |
| [SiteId](../../aspose.cells.metas/sensitivitylabel/siteid/) { get; set; } | يمثل معرّف موقع Azure Active Directory (Azure AD) المتعلق بسياسة تسمية الحساسية التي تصف تسمية الحساسية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            
            try
            {
                // إنشاء نسخة من فئة SensitivityLabel باستخدام الانعكاس
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // تعيين الخصائص الأساسية
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                label.ContentMarkType = SensitivityLabelMarkType.None;
                
                // عرض قيم الخصائص
                Console.WriteLine($"Sensitivity Label Created:");
                Console.WriteLine($"ID: {label.Id}");
                Console.WriteLine($"Enabled: {label.IsEnabled}");
                Console.WriteLine($"Assignment Type: {label.AssignmentType}");
                Console.WriteLine($"Content Mark Type: {label.ContentMarkType}");
                
                // احفظ المصنف
                workbook.Save("SensitivityLabelDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SensitivityLabel: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


