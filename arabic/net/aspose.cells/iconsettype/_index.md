---
title: "التعداد IconSetType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.IconSetType. نوع مجموعة الأيقونات للتنسيق الشرطي. قيم العتبة لتفعيل الأيقونات المختلفة داخل المجموعة قابلة للتكوين وترتيب الأيقونات قابل للعكس"
type: docs
url: /ar/net/aspose.cells/iconsettype/
---
## IconSetType enumeration

نوع مجموعة الأيقونات للتنسيق الشرطي. قيم العتبة لتفعيل الأيقونات المختلفة داخل المجموعة قابلة للتكوين، وترتيب الأيقونات قابل للعكس.

```csharp
public enum IconSetType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Arrows3 | `0` | مجموعة أيقونات 3 أسهم. |
| ArrowsGray3 | `1` | مجموعة أيقونات 3 أسهم رمادية. |
| Flags3 | `2` | مجموعة أيقونات 3 أعلام. |
| Signs3 | `3` | مجموعة أيقونات 3 إشارات. |
| Symbols3 | `4` | مجموعة أيقونات 3 رموز (مُحاطة بدائرة). |
| Symbols32 | `5` | مجموعة أيقونات 3 رموز (بدون دائرة). |
| TrafficLights31 | `6` | مجموعة أيقونات 3 إشارات ضوئية (بدون إطار). |
| TrafficLights32 | `7` | مجموعة أيقونات 3 إشارات ضوئية مع حد أسود سميك. |
| Arrows4 | `8` | مجموعة أيقونات 4 أسهم. |
| ArrowsGray4 | `9` | مجموعة أيقونات 4 أسهم رمادية. |
| Rating4 | `10` | مجموعة أيقونات 4 تقييمات. |
| RedToBlack4 | `11` | مجموعة أيقونات 4 'أحمر إلى أسود'. |
| TrafficLights4 | `12` | مجموعة أيقونات 4 إشارات ضوئية. |
| Arrows5 | `13` | مجموعة أيقونات أسهم 5. |
| ArrowsGray5 | `14` | مجموعة أيقونات أسهم رمادية 5. |
| Quarters5 | `15` | مجموعة أيقونات أرباع 5. |
| Rating5 | `16` | مجموعة أيقونات تقييم 5. |
| Stars3 | `17` | مجموعة نجوم 3 |
| Boxes5 | `18` | مجموعة صناديق 5 |
| Triangles3 | `19` | مجموعة مثلثات 3 |
| None | `20` | لا شيء |
| CustomSet | `21` | CustomSet. هذا العنصر للقراءة فقط. |
| Smilies3 | `22` | 3 رموز تعبيرية. فقط لملفات .ods. |
| ColorSmilies3 | `23` | 3 رموز تعبيرية ملونة. فقط لملفات .ods. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassIconSetTypeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // تعيين قيم عينة
            cells["A1"].PutValue(1);
            cells["A2"].PutValue("#DIV/0!");
            cells["A3"].PutValue(3);

            // إضافة تنسيق شرطي باستخدام مجموعة الأيقونات
            ConditionalFormattingCollection cfs = sheet.ConditionalFormattings;
            FormatConditionCollection fcs = cfs[cfs.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 3, 0));
            
            FormatCondition fc = fcs[fcs.AddCondition(FormatConditionType.IconSet)];
            fc.IconSet.Type = IconSetType.TrafficLights31;

            // احصل على النتائج وعرضها
            ConditionalFormattingResult res1 = cells["A1"].GetConditionalFormattingResult();
            Console.WriteLine($"A1 Icon Type: {res1.ConditionalFormattingIcon.Type}, Index: {res1.ConditionalFormattingIcon.Index}");

            ConditionalFormattingResult res3 = cells["A3"].GetConditionalFormattingResult();
            Console.WriteLine($"A3 Icon Type: {res3.ConditionalFormattingIcon.Type}, Index: {res3.ConditionalFormattingIcon.Index}");

            ConditionalFormattingResult res2 = cells["A2"].GetConditionalFormattingResult();
            Console.WriteLine($"A2 has formatting: {res2 != null && res2.ConditionalFormattingIcon != null}");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


