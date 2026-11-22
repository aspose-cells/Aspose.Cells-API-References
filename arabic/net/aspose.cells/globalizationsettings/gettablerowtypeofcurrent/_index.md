---
title: "GlobalizationSettings.GetTableRowTypeOfCurrent"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. تُحصل على اسم نوع صفوف الجدول التي تتكون من الصف الحالي في الجدول المرجعي. الافتراضي هو This Row لذا في الصيغة يمثل This Row الصف الحالي في الجدول المرجعي"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/gettablerowtypeofcurrent/
---
## GlobalizationSettings.GetTableRowTypeOfCurrent method

يحصل على اسم نوع صفوف الجدول التي تتكون من الصف الحالي في الجدول المشار إليه. الافتراضي هو "This Row"، لذا في الصيغة "#This Row" تمثل الصف الحالي في الجدول المشار إليه.

```csharp
public virtual string GetTableRowTypeOfCurrent()
```

### قيمة الإرجاع

اسم نوع صفوف الجدول

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class GlobalizationSettingsMethodGetTableRowTypeOfCurrentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين إعدادات العولمة المخصصة
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // إنشاء بيانات تجريبية وجدول
                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(2.5);
                worksheet.Cells["A3"].PutValue("Orange");
                worksheet.Cells["B3"].PutValue(1.8);

                // إنشاء جدول
                int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.DisplayName = "PriceTable"; // Fixed property name

                // إضافة صيغة باستخدام إشارة إلى الصف الحالي
                Cell formulaCell = worksheet.Cells["C2"];
                formulaCell.Formula = "=PriceTable[@Price] * 1.2";

                // توضيح تأثير GetTableRowTypeOfCurrent
                Console.WriteLine("Generated formula: " + formulaCell.Formula);
                Console.WriteLine("Method executed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfCurrent method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("MethodGetTableRowTypeOfCurrentDemo.xlsx");
        }
    }

    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetTableRowTypeOfCurrent()
        {
            return "CurrentItem"; // Custom current row identifier
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


