---
title: "تعداد InputMethodEditorMode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.ActiveXControls.InputMethodEditorMode. يمثل وضع التشغيل الافتراضي لمحرر طريقة الإدخال"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/inputmethodeditormode/
---
## InputMethodEditorMode enumeration

يمثل وضع التشغيل الافتراضي لمحرر طريقة الإدخال.

```csharp
public enum InputMethodEditorMode
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| NoControl | `0` | لا يتحكم في IME. |
| On | `1` | IME مُفعَّل. |
| Off | `2` | IME مُعطَّل. وضع الإنجليزية. |
| Disable | `3` | IME مُعطَّل. لا يمكن للمستخدم تشغيل IME عبر لوحة المفاتيح. |
| Hiragana | `4` | IME مُفعَّل بوضع هيراغانا بعرض كامل. |
| Katakana | `5` | IME مُفعَّل بوضع كاتاكانا بعرض كامل. |
| KatakanaHalf | `6` | IME مُفعَّل بوضع كاتاكانا بنصف عرض. |
| AlphaFull | `7` | IME مُفعَّل بوضع أبجدي رقمي بعرض كامل. |
| Alpha | `8` | IME مُفعَّل بوضع أبجدي رقمي بنصف عرض. |
| HangulFull | `9` | IME مُفعَّل بوضع هانغول بعرض كامل. |
| Hangul | `10` | IME مُفعَّل بوضع هانغول بنصف عرض. |
| HanziFull | `11` | IME مُفعَّل بوضع هانزي بعرض كامل. |
| Hanzi | `12` | IME مُفعَّل بوضع هانزي بنصف عرض. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class InputMethodEditorModeDemo
    {
        public static void InputMethodEditorModeExample()
        {
            // تهيئة دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة عنصر تحكم ActiveX TextBox إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // تعيين وضع IME إلى هيراغانا بعرض كامل
            textBoxControl.IMEMode = InputMethodEditorMode.Hiragana;

            // حدد خصائص أخرى للعرض
            textBoxControl.Text = "This is a test.";
            textBoxControl.IsEnabled = true;
            textBoxControl.IsLocked = false;
            textBoxControl.IsTransparent = false;
            textBoxControl.IsAutoSize = true;
            textBoxControl.Width = 200;
            textBoxControl.Height = 50;
            textBoxControl.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Black);
            textBoxControl.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.White);
            textBoxControl.IsVisible = true;
            textBoxControl.Shadow = false;

            // احفظ المصنف
            workbook.Save("InputMethodEditorModeExample.xlsx");
            workbook.Save("InputMethodEditorModeExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


