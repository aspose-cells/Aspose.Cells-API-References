---
title: "Style.IsModified"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Style. تتحقق مما إذا كانت الخصائص المحددة للنمط قد تم تعديلها. تُستخدم لنمط ConditionalFormattings للتحقق مما إذا كان يجب استخدام الخصائص المحددة لهذا النمط عند تطبيق ConditionalFormattings على خلية"
type: docs
url: /ar/net/aspose.cells/style/ismodified/
---
## Style.IsModified method

يتحقق مما إذا كانت الخصائص المحددة للنمط قد تم تعديلها. يُستخدم لنمط ConditionalFormattings للتحقق مما إذا كان يجب استخدام الخصائص المحددة لهذا النمط عند تطبيق ConditionalFormattings على خلية.

```csharp
public bool IsModified(StyleModifyFlag modifyFlag)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| modifyFlag | StyleModifyFlag | علامات تعديل النمط |

### قيمة الإرجاع

صحيح إذا تم تعديل الخصائص المحددة

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleMethodIsModifiedWithStyleModifyFlagDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احصل على نمط الخلية A1
            Style style = worksheet.Cells["A1"].GetStyle();
            
            // تعديل النمط (الخلفية) للستايل
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            
            // تحقق مما إذا تم تعديل النمط
            bool isPatternModified = style.IsModified(StyleModifyFlag.Pattern);
            
            // أخرج النتيجة.
            Console.WriteLine("Is pattern modified: " + isPatternModified);
        }
    }
}
```

### انظر أيضًا

* enum [StyleModifyFlag](../../stylemodifyflag/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


