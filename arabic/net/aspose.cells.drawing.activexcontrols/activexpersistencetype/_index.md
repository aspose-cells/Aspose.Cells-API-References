---
title: "تعداد ActiveXPersistenceType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.ActiveXControls.ActiveXPersistenceType. يمثل طريقة الاستمرارية لحفظ عنصر تحكم ActiveX"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/activexpersistencetype/
---
## ActiveXPersistenceType enumeration

يمثل طريقة الاستمرار لحفظ عنصر تحكم ActiveX.

```csharp
public enum ActiveXPersistenceType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| PropertyBag | `0` | يتم تخزين البيانات كبيانات xml. |
| Storage | `1` | يتم تخزين البيانات كبيانات ثنائية للتخزين. |
| Stream | `2` | يتم تخزين البيانات كبيانات ثنائية للتدفق. |
| StreamInit | `3` | يتم تخزين البيانات كبيانات ثنائية لـ streaminit. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlsClassActiveXPersistenceTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cells cells = worksheet.Cells;
            cells["A2"].Value = "Sales";
            cells["A3"].Value = "Finance";
            cells["A4"].Value = "MIS";
            cells["A5"].Value = "R&D";
            cells["A6"].Value = "Marketing";
            cells["A7"].Value = "HRA";

            // أضف عناصر تحكم ActiveX مختلفة لتوضيح أنواع الاستمرارية المختلفة.
            AddControlWithPersistenceType(worksheet, ControlType.CommandButton, ActiveXPersistenceType.PropertyBag, 0, 2);
            AddControlWithPersistenceType(worksheet, ControlType.TextBox, ActiveXPersistenceType.Storage, 4, 2);
            AddControlWithPersistenceType(worksheet, ControlType.CheckBox, ActiveXPersistenceType.Stream, 8, 2);
            AddControlWithPersistenceType(worksheet, ControlType.ComboBox, ActiveXPersistenceType.StreamInit, 12, 2);

            // احفظ دفتر العمل مع جميع عناصر تحكم ActiveX.
            workbook.Save("ActiveXPersistenceTypeDemo.xlsx");
        }

        private static void AddControlWithPersistenceType(Worksheet worksheet, ControlType controlType,
            ActiveXPersistenceType persistenceType, int row, int column)
        {
            // أضف عنصر تحكم ActiveX.
            Shape shape = worksheet.Shapes.AddActiveXControl(
                controlType,
                row,
                15,
                column,
                15,
                200,
                50
            );

            // قم بتكوين العنصر بناءً على النوع.
            switch (controlType)
            {
                case ControlType.CommandButton:
                    var button = (CommandButtonActiveXControl)shape.ActiveXControl;
                    button.IsVisible = true;
                    
                    button.Caption = $"{persistenceType} Button";
                    break;

                case ControlType.TextBox:
                    var textBox = (TextBoxActiveXControl)shape.ActiveXControl;
                    textBox.IsVisible = true;
                    textBox.Text = $"{persistenceType} TextBox";
                    break;

                case ControlType.CheckBox:
                    var checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;
                    checkBox.IsVisible = true;
                    checkBox.Caption = $"{persistenceType} CheckBox";
                    checkBox.Value = CheckValueType.Checked;
                    break;

                case ControlType.ComboBox:
                    var comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;
                    comboBox.IsVisible = true;
                    comboBox.ListFillRange = $"A3:A7";
                    break;
            }

            // يتم معالجة نوع الاستمرارية داخليًا بواسطة Aspose.Cells عند الحفظ.
            Console.WriteLine($"Added {controlType} with persistence type: {persistenceType}");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


