---
title: "SensitivityLabel.ContentMarkType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SensitivityLabel. تحصل وتعيّن أنواع وضع العلامات على المحتوى التي يجب تطبيقها على الملف"
type: docs
url: /ar/net/aspose.cells.metas/sensitivitylabel/contentmarktype/
---
## SensitivityLabel.ContentMarkType property

يحصل على ويضبط أنواع تمييز المحتوى التي يجب تطبيقها على ملف.

```csharp
public SensitivityLabelMarkType ContentMarkType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class SensitivityLabelPropertyContentMarkTypeDemo
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
                
                // عرض خاصية ContentMarkType (قراءة-كتابة)
                Console.WriteLine("Initial ContentMarkType: " + label.ContentMarkType);
                
                // تعيين أنواع مختلفة من وضع العلامات على المحتوى
                label.ContentMarkType = SensitivityLabelMarkType.Header;
                Console.WriteLine("After setting Header: " + label.ContentMarkType);
                
                label.ContentMarkType = SensitivityLabelMarkType.Watermark;
                Console.WriteLine("After setting Watermark: " + label.ContentMarkType);
                
                // عرض استخدام العلامات المدمجة
                label.ContentMarkType = SensitivityLabelMarkType.Header | SensitivityLabelMarkType.Footer;
                Console.WriteLine("Combined Header+Footer: " + label.ContentMarkType);
                
                // احفظ المصنف
                workbook.Save("ContentMarkTypeDemo.xlsx");
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

* enum [SensitivityLabelMarkType](../../sensitivitylabelmarktype/)
* class [SensitivityLabel](../)
* namespace [Aspose.Cells.Metas](../../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../../)


