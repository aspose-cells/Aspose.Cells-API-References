---
title: "RadioButton.GetOptionIndex"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة RadioButton. تحصل على فهرس الخيار (مبني على الواحد) في جميع أزرار الاختيار داخل GroupBox الذي يحتوي على زر الاختيار هذا"
type: docs
url: /ar/net/aspose.cells.drawing/radiobutton/getoptionindex/
---
## RadioButton.GetOptionIndex method

يحصل على فهرس الخيار (مبني على الواحد) في جميع أزرار الاختيار داخل GroupBox الذي يحتوي على هذا الزر.

```csharp
public int GetOptionIndex()
```

### ملاحظات

إذا لم يكن زر الاختيار هذا داخل GroupBox، تُعيد فهرس الخيار في جميع أزرار الاختيار التي ليست داخل أي GroupBox

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class RadioButtonMethodGetOptionIndexDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة GroupBox لاحتواء أزرار الراديو
            GroupBox groupBox = worksheet.Shapes.AddGroupBox(1, 0, 100, 200, 100, 200);

            // إضافة ثلاثة أزرار اختيار إلى GroupBox
            RadioButton radioButton1 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 20, 100, 20, 100);
            RadioButton radioButton2 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 50, 100, 20, 100);
            RadioButton radioButton3 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 80, 100, 20, 100);

            // تعيين أزرار الاختيار لتكون جزءًا من GroupBox
            radioButton1.Placement = PlacementType.FreeFloating;
            radioButton2.Placement = PlacementType.FreeFloating;
            radioButton3.Placement = PlacementType.FreeFloating;

            try
            {
                // الحصول على فهرس الخيار لكل زر اختيار
                int index1 = radioButton1.GetOptionIndex();
                int index2 = radioButton2.GetOptionIndex();
                int index3 = radioButton3.GetOptionIndex();

                Console.WriteLine($"RadioButton1 Option Index: {index1}");
                Console.WriteLine($"RadioButton2 Option Index: {index2}");
                Console.WriteLine($"RadioButton3 Option Index: {index3}");

                // تحديد زر الاختيار الأول لتوضيح الاختيار
                radioButton1.IsChecked = true;
                Console.WriteLine("RadioButton1 is checked");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOptionIndex method: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("RadioButtonMethodGetOptionIndexDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


