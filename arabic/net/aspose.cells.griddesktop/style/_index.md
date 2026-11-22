---
title: "فئة Style"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridDesktop.Style. تمثل نمط العرض لمستندات Excel مثل لون الخط والمحاذاة والحدود إلخ"
type: docs
url: /ar/net/aspose.cells.griddesktop/style/
---
## Style class

يمثل نمط العرض لمستند إكسل، مثل الخط، اللون، المحاذاة، الحدود، إلخ.

```csharp
public class Style
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [Style](style/)(GridDesktop) | إنشاء Style جديد للتحكم |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [BackgroundColor](../../aspose.cells.griddesktop/style/backgroundcolor/) { get; set; } | يحصل أو يضبط لون خلفية الخلية، إذا لم يتم تعيين نمط النمط إلى صلب، فسيتم تطبيقه |
| [CellLocked](../../aspose.cells.griddesktop/style/celllocked/) { get; set; } | يحصل على قيمة أو يضبطها تشير إلى ما إذا كان يمكن تعديل الخلية أم لا. |
| [Color](../../aspose.cells.griddesktop/style/color/) { get; set; } | يحصل أو يضبط لون تظليل الخلية. عندما يكون النمط none، يرجع Color.Empty؛ عندما يكون النمط BackgroundType.Solid، يرجع ForegroundColor؛ غير ذلك يرجع BackgroundColor |
| [Custom](../../aspose.cells.griddesktop/style/custom/) { get; set; } | يمثل سلسلة تنسيق الرقم المخصص لهذا الكائن من النوع Style. إذا لم يتم تعيين تنسيق الرقم المخصص (على سبيل المثال، إذا كان تنسيق الرقم مدمجًا)، سيتم إرجاع "". |
| [Font](../../aspose.cells.griddesktop/style/font/) { get; set; } | يحصل على كائن [`GridFont`](../../aspose.cells.griddesktop.data/gridfont/) . |
| [ForegroundColor](../../aspose.cells.griddesktop/style/foregroundcolor/) { get; set; } | يحصل على لون الأمام للنمط أو يضبطه. |
| [HAlignment](../../aspose.cells.griddesktop/style/halignment/) { get; set; } | يحصل أو يضبط سمة المحاذاة الأفقية. |
| [Indent](../../aspose.cells.griddesktop/style/indent/) { get; set; } | يمثل مستوى m_IndentLevel للخلية أو النطاق. يمكن أن يكون عددًا صحيحًا فقط من 0 إلى 15. |
| [NumberType](../../aspose.cells.griddesktop/style/numbertype/) { get; set; } | يحصل على تنسيق العرض للأرقام والتواريخ أو يضبطه. أنماط التنسيق تختلف بين المناطق المختلفة. |
| [Pattern](../../aspose.cells.griddesktop/style/pattern/) { get; set; } | يحصل على نوع نمط خلفية الخلية أو يضبطه. |
| [Rotation](../../aspose.cells.griddesktop/style/rotation/) { get; set; } | يمثل زاوية دوران النص. |
| [Shrink](../../aspose.cells.griddesktop/style/shrink/) { get; set; } | يمثل ما إذا كان النص يتقلص تلقائيًا ليتناسب مع عرض العمود المتاح. |
| [TextDirection](../../aspose.cells.griddesktop/style/textdirection/) { get; set; } | يحصل أو يضبط سمة اتجاه النص. |
| [TextWrapped](../../aspose.cells.griddesktop/style/textwrapped/) { get; set; } | يحصل على قيمة أو يضبطها تشير إلى ما إذا كان النص داخل الخلية مُلتفًا. |
| [VAlignment](../../aspose.cells.griddesktop/style/valignment/) { get; set; } | يحصل أو يضبط سمة المحاذاة العمودية. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Clone](../../aspose.cells.griddesktop/style/clone/)() | ينشئ ويعيد نسخة من هذا الكائن. **NOTE:** إذا قمت باستنساخ نمط مسمى، فإن الاسم لا يتم استنساخه لأن اسم النمط يجب أن يكون فريدًا. لذلك، النمط المستنسخ لن يكون "equals to" النمط الأصلي. |
| [SetBorderColor](../../aspose.cells.griddesktop/style/setbordercolor/)(BorderType, Color) | يضبط لون الحد المحدد. |
| [SetBorderLine](../../aspose.cells.griddesktop/style/setborderline/)(BorderType, BorderLineType) | يضبط نوع خط الحد للحد المحدد. |

### انظر أيضًا

* namespace [Aspose.Cells.GridDesktop](../../aspose.cells.griddesktop/)
* assembly [Aspose.Cells.GridDesktop](../../)


