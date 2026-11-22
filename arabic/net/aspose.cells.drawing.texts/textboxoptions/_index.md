---
title: "فئة TextBoxOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.Texts.TextBoxOptions class. يمثل خيارات النص للشكل"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textboxoptions/
---
## TextBoxOptions class

يمثل خيارات نص الشكل

```csharp
public class TextBoxOptions
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AllowTextToOverflow](../../aspose.cells.drawing.texts/textboxoptions/allowtexttooverflow/) { get; set; } | ما إذا كان يُسمح للنص بتجاوز الشكل. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/textboxoptions/bottommarginpt/) { get; set; } | يعيد الهامش السفلي بوحدة النقاط |
| [LeftMarginPt](../../aspose.cells.drawing.texts/textboxoptions/leftmarginpt/) { get; set; } | يحصل ويضبط الهامش الأيسر بوحدة نقاط. |
| [ResizeToFitText](../../aspose.cells.drawing.texts/textboxoptions/resizetofittext/) { get; set; } | يشير إلى ما إذا كان يجب تغيير حجم الشكل ليتناسب مع النص |
| [RightMarginPt](../../aspose.cells.drawing.texts/textboxoptions/rightmarginpt/) { get; set; } | يحصل ويضبط الهامش الأيمن بوحدة نقاط. |
| [ShapeTextDirection](../../aspose.cells.drawing.texts/textboxoptions/shapetextdirection/) { get; set; } | يحصل أو يضبط اتجاه عرض النص داخل جسم نص معين. يتطابق مع "Format Shape - Text Options - Text Box - Text direction" في Excel |
| [ShapeTextVerticalAlignment](../../aspose.cells.drawing.texts/textboxoptions/shapetextverticalalignment/) { get; set; } | يتطابق مع "Format Shape - Text Options - Text Box - Vertical Alignment" في Excel. |
| [TopMarginPt](../../aspose.cells.drawing.texts/textboxoptions/topmarginpt/) { get; set; } | يحصل ويضبط الهامش العلوي بوحدة نقاط. |
| [WrapTextInShape](../../aspose.cells.drawing.texts/textboxoptions/wraptextinshape/) { get; set; } | يحدد تغليف النص داخل الشكل. False - لن يحدث تغليف على جسم النص. True - سيحدث تغليف على جسم النص. |

### أمثلة

```csharp

[C#]
//إنشاء كائن Workbook
Workbook workbook = new Workbook();
int index = workbook.Worksheets[0].TextBoxes.Add(0, 0, 350, 350);
Shape shape = workbook.Worksheets[0].TextBoxes[index];
shape.Text = "This is test.";

//قم بأعمالك

//احفظ ملف Excel.
workbook.Save("exmaple.xlsx");
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


