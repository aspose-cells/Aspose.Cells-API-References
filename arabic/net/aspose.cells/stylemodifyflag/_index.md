---
title: "التعداد StyleModifyFlag"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.StyleModifyFlag. علامات تعديل النمط"
type: docs
url: /ar/net/aspose.cells/stylemodifyflag/
---
## StyleModifyFlag enumeration

علامات تعديل النمط.

```csharp
public enum StyleModifyFlag
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| LeftBorder | `256` | يشير إلى ما إذا كان الحد الأيسر قد تم تعديله للنمط. |
| RightBorder | `512` | يشير إلى ما إذا كان الحد الأيمن قد تم تعديله للنمط. |
| TopBorder | `1024` | يشير إلى ما إذا كان الحد العلوي قد تم تعديله للنمط. |
| BottomBorder | `2048` | يشير إلى ما إذا كان الحد السفلي قد تم تعديله للنمط. |
| DiagonalDownBorder | `4096` | يشير إلى ما إذا كان الحد القطري السفلي قد تم تعديله للنمط. |
| DiagonalUpBorder | `8192` | يشير إلى ما إذا كان الحد القطري العلوي قد تم تعديله للنمط. |
| HorizontalBorder | `32` | يشير إلى ما إذا كان الحد الأفقي قد تم تعديله للنمط. فقط للنمط الديناميكي، مثل التنسيق الشرطي. |
| VerticalBorder | `64` | يشير إلى ما إذا كان الحد العمودي قد تم تعديله للنمط. فقط للنمط الديناميكي، مثل التنسيق الشرطي. |
| SideBorders | `3840` | يشير إلى حدود الأربعة الجوانب: LeftBorder، RightBorder، TopBorder و BottomBorder. |
| Diagonal | `12288` | يشير إلى الحدود القطرية: DiagonalDownBorder و DiagonalUpBorder. |
| DynamicStyleBorders | `96` | يشير إلى حدود النمط الديناميكي: HorizontalBorder و VerticalBorder. |
| Borders | `16224` | يشير إلى ما إذا كان حد واحد أو أكثر (LeftBorder، RightBorder، TopBorder، BottomBorder، Diagonal، HorizontalBorder، VerticalBorder) قد تم تعديله للنمط. |
| NumberFormat | `16384` | يشير إلى ما إذا تم تعديل numberformat. |
| HorizontalAlignment | `32768` | يشير إلى ما إذا تم تعديل horizontal alignment. |
| VerticalAlignment | `65536` | يشير إلى ما إذا تم تعديل vertical alignment. |
| Indent | `131072` | يشير إلى ما إذا تم تعديل خاصية indent. |
| Rotation | `262144` | يشير إلى ما إذا تم تعديل خاصية rotation. |
| WrapText | `524288` | يشير إلى ما إذا تم تعديل خاصية wrap text. |
| ShrinkToFit | `1048576` | يشير إلى ما إذا تم تعديل خاصية shrink to fit. |
| TextDirection | `2097152` | يشير إلى ما إذا تم تعديل خاصية text direction. |
| RelativeIndent | `128` | يشير إلى ما إذا تم تعديل خاصية relative indent للنمط. فقط للنمط الديناميكي، مثل التنسيق الشرطي. |
| AlignmentSettings | `4161664` | يشير إلى ما إذا تم تعديل خاصية أو أكثر مرتبطة بالمحاذاة (HorizontalAlignment, VerticalAlignment, Rotation, WrapText, WrapText, Indent, ShrinkToFit, TextDirection, RelativeIndent). |
| Pattern | `4194304` | يشير إلى ما إذا تم تعديل نمط التظليل. |
| ForegroundColor | `8388608` | يشير إلى ما إذا تم تعديل لون المقدمة. |
| BackgroundColor | `16777216` | يشير إلى ما إذا تم تعديل لون الخلفية. |
| CellShading | `29360128` | يشير إلى ما إذا تم تعديل خاصية أو أكثر مرتبطة بالتظليل (Pattern, ForegroundColor, BackgroundColor). |
| Locked | `67108864` | يشير إلى ما إذا تم تعديل خاصية locked. |
| HideFormula | `134217728` | يشير إلى ما إذا تم تعديل hide formula. |
| ProtectionSettings | `201326592` | يشير إلى ما إذا تم تعديل خاصية أو أكثر مرتبطة بالحماية (Locked, HideFormula). |
| FontSize | `1` | يشير إلى ما إذا تم تعديل حجم الخط. |
| FontName | `2` | يشير إلى ما إذا تم تعديل اسم الخط. |
| FontColor | `3` | يشير إلى ما إذا تم تعديل لون الخط. |
| FontWeight | `4` | يشير إلى ما إذا تم تعديل وزن الخط. |
| FontItalic | `5` | يشير إلى ما إذا تم تعديل خاصية italic للخط. |
| FontUnderline | `6` | يشير إلى ما إذا تم تعديل خاصية underline للخط. |
| FontStrike | `7` | يشير إلى ما إذا تم تعديل خاصية strike للخط. |
| FontScript | `8` | يشير إلى ما إذا تم تعديل خاصية subscript أو superscript للخط. |
| FontFamily | `9` | يشير إلى ما إذا تم تعديل عائلة الخط. |
| FontCharset | `10` | يشير إلى ما إذا تم تعديل مجموعة الأحرف للخط. |
| FontScheme | `11` | غير مستخدم. |
| FontDirty | `12` | غير مستخدم. |
| FontSpellingError | `13` | غير مستخدم. |
| FontUFillTx | `14` | غير مستخدم. |
| FontSpacing | `15` | غير مستخدم. |
| FontKerning | `16` | غير مستخدم. |
| FontEqualize | `17` | غير مستخدم. |
| FontCap | `18` | غير مستخدم. |
| FontVerticalText | `19` |  |
| Font | `31` | يشير إلى ما إذا تم تعديل خاصية أو أكثر لخط النمط. |
| All | `234881023` | جميع الخصائص التي يمكن تعديلها للنمط. |
| None | `0` | لم يتم تحديد أي خاصية. |

### ملاحظات

تم تعريف تركيبات متعددة من الخصائص لتسهيل الاستخدام. عند التحقق مما إذا تم تعديلها لنمط واحد، تشير القيمة المرجعة إلى ما إذا تم تعديل خاصية واحدة أو أكثر في التركيبة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleModifyFlagDemo
    {
        public static void StyleModifyFlagExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين بعض القيم في ورقة العمل
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["A2"].PutValue(123.45);

            // إنشاء نمط جديد
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.Color = System.Drawing.Color.Blue;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.VerticalAlignment = TextAlignmentType.Center;

            // تطبيق النمط على خلية
            worksheet.Cells["A1"].SetStyle(style);

            // تحقق من الخصائص التي تم تعديلها في النمط
            bool isFontModified = style.IsModified(StyleModifyFlag.Font);
            bool isFontSizeModified = style.IsModified(StyleModifyFlag.FontSize);
            bool isFontColorModified = style.IsModified(StyleModifyFlag.FontColor);
            bool isHorizontalAlignmentModified = style.IsModified(StyleModifyFlag.HorizontalAlignment);

            // أخرج النتائج
            Console.WriteLine("Font Modified: " + isFontModified);
            Console.WriteLine("Font Size Modified: " + isFontSizeModified);
            Console.WriteLine("Font Color Modified: " + isFontColorModified);
            Console.WriteLine("Horizontal Alignment Modified: " + isHorizontalAlignmentModified);

            // احفظ المصنف
            workbook.Save("StyleModifyFlagExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


