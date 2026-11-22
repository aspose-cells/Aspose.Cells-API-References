---
title: "HtmlSaveOptions.ExcludeUnusedStyles"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان سيتم استبعاد الأنماط غير المستخدمة. استبعاد الأنماط غير المستخدمة في ملفات HTML المولدة يمكن أن يقلل حجم الملف دون التأثير على التأثيرات البصرية. لذلك القيمة الافتراضية لهذه الخاصية هي true. إذا كان المستخدم يحتاج إلى الاحتفاظ بجميع الأنماط في المصنف للـ HTML المولد، مثل السيناريو الذي يحتاج فيه المستخدم إلى استعادة المصنف من الـ HTML المولد لاحقًا، يرجى تعيين هذه الخاصية إلى false."
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/excludeunusedstyles/
---
## HtmlSaveOptions.ExcludeUnusedStyles property

يشير إلى ما إذا كان يتم استبعاد الأنماط غير المستخدمة. بالنسبة لملفات html المولدة، استبعاد الأنماط غير المستخدمة يمكن أن يقلل حجم الملف دون التأثير على التأثيرات البصرية. لذا القيمة الافتراضية لهذه الخاصية هي true. إذا كان المستخدم يحتاج إلى الاحتفاظ بجميع الأنماط في المصنف للـ html المولد (مثل السيناريو الذي يحتاج فيه المستخدم لاستعادة المصنف من الـ html المولد لاحقًا)، يرجى تعيين هذه الخاصية إلى false.

```csharp
public bool ExcludeUnusedStyles { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExcludeUnusedStylesDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // إضافة بيانات نموذجية بأنماط مختلفة
            Cell cell1 = workbook.Worksheets[0].Cells["A1"];
            cell1.Value = "Styled text";
            Style style1 = cell1.GetStyle();
            style1.Font.Color = Color.Red;
            style1.Font.IsBold = true;
            cell1.SetStyle(style1);

            Cell cell2 = workbook.Worksheets[0].Cells["A2"];
            cell2.Value = "Different style";
            Style style2 = cell2.GetStyle();
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            cell2.SetStyle(style2);

            // تكوين خيارات حفظ HTML لاستبعاد الأنماط غير المستخدمة
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExcludeUnusedStyles = true;

            // حفظ دفتر العمل مع خيارات HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            Console.WriteLine("HTML file saved with ExcludeUnusedStyles=true");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


