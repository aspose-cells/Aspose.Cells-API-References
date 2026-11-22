---
title: "تعداد ControlBorderType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.ActiveXControls.ControlBorderType. يمثل نوع الحدود لعنصر التحكم ActiveX"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/controlbordertype/
---
## ControlBorderType enumeration

يمثل نوع الحد للتحكم ActiveX.

```csharp
public enum ControlBorderType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | بدون حدود. |
| Single | `1` | السطر المفرد. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;

    public class ControlBorderTypeDemo
    {
        public static void ControlBorderTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف عنصر تحكم ComboBox ActiveX إلى ورقة العمل
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // ضبط الخصائص لعنصر تحكم ActiveX من نوع ComboBox
            comboBox.MaxLength = 100;
            comboBox.ListWidth = 150;
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = 1;
            comboBox.ColumnCount = 1;
            comboBox.ListRows = 5;
            comboBox.MatchEntry = ControlMatchEntryType.Complete;
            comboBox.DropButtonStyle = DropButtonStyle.Arrow;
            comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Always;
            comboBox.ListStyle = ControlListStyle.Plain;
            comboBox.BorderStyle = ControlBorderType.Single; // Set border style to Single
            comboBox.BorderOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Black);
            comboBox.SpecialEffect = ControlSpecialEffectType.Flat;
            comboBox.IsEditable = true;
            comboBox.ShowColumnHeads = false;
            comboBox.IsDragBehaviorEnabled = false;
            comboBox.EnterFieldBehavior = true;
            comboBox.IsAutoWordSelected = false;
            comboBox.SelectionMargin = false;
            comboBox.Value = "Sample Text";
            comboBox.HideSelection = true;
            comboBox.ColumnWidths = 100;

            // احفظ المصنف
            workbook.Save("ControlBorderTypeExample.xlsx");
            workbook.Save("ControlBorderTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


