---
title: "التعداد ControlMatchEntryType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.ActiveXControls.ControlMatchEntryType. يوضح كيفية بحث ListBox أو ComboBox في قائمته أثناء كتابة المستخدم"
type: docs
url: /ar/net/aspose.cells.drawing.activexcontrols/controlmatchentrytype/
---
## ControlMatchEntryType enumeration

يمثل طريقة بحث ListBox أو ComboBox في قائمته أثناء كتابة المستخدم.

```csharp
public enum ControlMatchEntryType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| FirstLetter | `0` | يبحث التحكم عن الإدخال التالي الذي يبدأ بالحرف المدخل. كتابة الحرف نفسه مرارًا وتكرارًا تتنقل عبر جميع الإدخالات التي تبدأ بهذا الحرف. |
| Complete | `1` | مع كتابة كل حرف، يبحث التحكم عن إدخال يطابق جميع الأحرف المدخلة. |
| None | `2` | لن يتم البحث في القائمة عند كتابة الأحرف. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ControlMatchEntryTypeDemo
    {
        public static void ControlMatchEntryTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // أضف عنصر تحكم ComboBox ActiveX إلى ورقة العمل
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // حدد الخصائص لـ ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 3;
            comboBox.ColumnCount = 1;
            comboBox.MatchEntry = ControlMatchEntryType.Complete; // Set the MatchEntry type to Complete
            comboBox.IsEditable = true;

            // إضافة عناصر إلى ComboBox
            comboBox.Value = "Apple;Banana;Cherry";

            // إضافة عنصر تحكم ListBox ActiveX إلى ورقة العمل
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 10, 0, 1, 0, 100, 60);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape2.ActiveXControl;

            // ضبط الخصائص لـ ListBox
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            listBox.MatchEntry = ControlMatchEntryType.FirstLetter; // Set the MatchEntry type to FirstLetter
            listBox.SelectionType = SelectionType.Single;

            // إضافة عناصر إلى ListBox
            listBox.Value = "Apple;Banana;Cherry";

            // احفظ المصنف
            workbook.Save("ControlMatchEntryTypeExample.xlsx");
            workbook.Save("ControlMatchEntryTypeExample.pdf");

            // أخرج النتائج
            Console.WriteLine("ComboBox and ListBox with different MatchEntry types have been created and saved to ControlMatchEntryTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


