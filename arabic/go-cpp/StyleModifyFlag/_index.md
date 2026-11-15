---
title: "تعداد StyleModifyFlag"
linktitle: "StyleModifyFlag"
second_title: "مرجع API لـ Aspose.Cells for Go عبر C++"
description: "تعداد StyleModifyFlag. يغلف الكائن الذي يمثل stylemodifyflag في Go."
type: docs
weight: 200
url: /ar/go-cpp/stylemodifyflag/
---

## StyleModifyFlag Enum

علامات تعديل النمط.

```go

type StyleModifyFlag int32


```

## الحقول

| حقل | الوصف |
| --- | --- |
| [LeftBorder](./leftborder/) | يشير إلى ما إذا كان الحد الأيسر قد تم تعديله للنمط. |
| [RightBorder](./rightborder/) | يشير إلى ما إذا كان الحد الأيمن قد تم تعديله للنمط. |
| [TopBorder](./topborder/) | يشير إلى ما إذا كان الحد العلوي قد تم تعديله للنمط. |
| [BottomBorder](./bottomborder/) | يشير إلى ما إذا كان الحد السفلي قد تم تعديله للنمط. |
| [DiagonalDownBorder](./diagonaldownborder/) | يشير إلى ما إذا كان الحد القطري-النازل قد تم تعديله للنمط. |
| [DiagonalUpBorder](./diagonalupborder/) | يشير إلى ما إذا كان الحد القطري-الصاعد قد تم تعديله للنمط. |
| [HorizontalBorder](./horizontalborder/) | يشير إلى ما إذا كان الحد الأفقي قد تم تعديله للنمط. فقط للأنماط الديناميكية، مثل التنسيق الشرطي. |
| [VerticalBorder](./verticalborder/) | يشير إلى ما إذا كان الحد العمودي قد تم تعديله للنمط. فقط للأنماط الديناميكية، مثل التنسيق الشرطي. |
| [SideBorders](./sideborders/) | يشير إلى حدود الأربعة الجوانب: <see cref=\"LeftBorder\"/>,<see cref=\"RightBorder\"/>, <see cref=\"TopBorder\"/> و <see cref=\"BottomBorder\"/>. |
| [Diagonal](./diagonal/) | يشير إلى الحدود القطرية: <see cref=\"DiagonalDownBorder\"/> و <see cref=\"DiagonalUpBorder\"/>. |
| [DynamicStyleBorders](./dynamicstyleborders/) | يشير إلى حدود النمط الديناميكي: <see cref=\"HorizontalBorder\"/> و <see cref=\"VerticalBorder\"/>. |
| [Borders](./borders/) | يشير إلى ما إذا كان حد واحد أو أكثر (<see cref=\"LeftBorder\"/>,<see cref=\"RightBorder\"/>, <see cref=\"TopBorder\"/>, <see cref=\"BottomBorder\"/>,<see cref=\"Diagonal\"/>, <see cref=\"HorizontalBorder\"/>, <see cref=\"VerticalBorder\"/>) قد تم تعديله للنمط. |
| [NumberFormat](./numberformat/) | يشير إلى ما إذا كان تنسيق الرقم قد تم تعديله. |
| [HorizontalAlignment](./horizontalalignment/) | يشير إلى ما إذا تم تعديل المحاذاة الأفقية. |
| [VerticalAlignment](./verticalalignment/) | يشير إلى ما إذا تم تعديل المحاذاة العمودية. |
| [Indent](./indent/) | يشير إلى ما إذا تم تعديل خاصية المسافة البادئة. |
| [Rotation](./rotation/) | يشير إلى ما إذا تم تعديل خاصية الدوران. |
| [WrapText](./wraptext/) | يشير إلى ما إذا تم تعديل خاصية لف النص. |
| [ShrinkToFit](./shrinktofit/) | يشير إلى ما إذا تم تعديل خاصية التصغير لتناسب. |
| [TextDirection](./textdirection/) | يشير إلى ما إذا تم تعديل خاصية اتجاه النص. |
| [RelativeIndent](./relativeindent/) | يشير إلى ما إذا تم تعديل خاصية المسافة البادئة النسبية للنمط. فقط للأنماط الديناميكية، مثل التنسيق الشرطي. |
| [AlignmentSettings](./alignmentsettings/) | يشير إلى ما إذا تم تعديل خاصية أو أكثر متعلقة بالمحاذاة (<see cref="HorizontalAlignment"/>,<see cref="VerticalAlignment"/>, <see cref="Rotation"/>, <see cref="WrapText"/>,<see cref="WrapText"/>, <see cref="Indent"/>, <see cref="ShrinkToFit"/>, <see cref="TextDirection"/>,<see cref="RelativeIndent"/>) |
| [Pattern](./pattern/) | يشير إلى ما إذا تم تعديل نمط التظليل. |
| [ForegroundColor](./foregroundcolor/) | يشير إلى ما إذا تم تعديل لون المقدمة. |
| [BackgroundColor](./backgroundcolor/) | يشير إلى ما إذا تم تعديل لون الخلفية. |
| [CellShading](./cellshading/) | يشير إلى ما إذا تم تعديل خاصية أو أكثر متعلقة بالتظليل (<see cref="Pattern"/>,<see cref="ForegroundColor"/>, <see cref="BackgroundColor"/>) |
| [Locked](./locked/) | يشير إلى ما إذا تم تعديل خاصية القفل. |
| [HideFormula](./hideformula/) | يشير إلى ما إذا تم تعديل إخفاء الصيغة. |
| [ProtectionSettings](./protectionsettings/) | يشير إلى ما إذا تم تعديل خاصية أو أكثر متعلقة بالحماية (<see cref="Locked"/>,<see cref="HideFormula"/>) |
| [FontSize](./fontsize/) | يشير إلى ما إذا تم تعديل حجم الخط. |
| [FontName](./fontname/) | يشير إلى ما إذا تم تعديل اسم الخط. |
| [FontColor](./fontcolor/) | يشير إلى ما إذا تم تعديل لون الخط. |
| [FontWeight](./fontweight/) | يشير إلى ما إذا تم تعديل وزن الخط. |
| [FontItalic](./fontitalic/) | يشير إلى ما إذا تم تعديل خاصية الخط المائل. |
| [FontUnderline](./fontunderline/) | يشير إلى ما إذا تم تعديل خاصية تسطير الخط. |
| [FontStrike](./fontstrike/) | يشير إلى ما إذا تم تعديل خاصية الخط المشطوب. |
| [FontScript](./fontscript/) | يشير إلى ما إذا تم تعديل خاصية الخط تحت السطر أو فوق السطر. |
| [FontFamily](./fontfamily/) | يشير إلى ما إذا تم تعديل عائلة الخط. |
| [FontCharset](./fontcharset/) | يشير إلى ما إذا تم تعديل مجموعة الأحرف للخط. |
| [FontScheme](./fontscheme/) | غير مستخدم. |
| [FontDirty](./fontdirty/) | غير مستخدم. |
| [FontSpellingError](./fontspellingerror/) | غير مستخدم. |
| [FontUFillTx](./fontufilltx/) | غير مستخدم. |
| [FontSpacing](./fontspacing/) | غير مستخدم. |
| [FontKerning](./fontkerning/) | غير مستخدم. |
| [FontEqualize](./fontequalize/) | غير مستخدم. |
| [FontCap](./fontcap/) | غير مستخدم. |
|[FontVerticalText](./fontverticaltext/) |  | 
| [Font](./font/) | يشير إلى ما إذا تم تعديل خاصية واحدة أو أكثر لخط النمط. |
| [All](./all/) | جميع الخصائص التي يمكن تعديلها للنمط. |
| [None](./none/) | لم يتم تحديد أي خاصية. |
