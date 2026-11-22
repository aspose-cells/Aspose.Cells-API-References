---
title: "GlobalizationSettings.GetDefaultSheetName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. تحصل على اسم الورقة الافتراضي لإضافة ورقة عمل تلقائيًا. الافتراضي هو Sheet"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/getdefaultsheetname/
---
## GlobalizationSettings.GetDefaultSheetName method

يحصل على اسم الورقة الافتراضي لإضافة ورقة العمل تلقائيًا. الافتراضي هو "Sheet".

```csharp
public virtual string GetDefaultSheetName()
```

### قيمة الإرجاع

اسم الورقة الافتراضي لإضافة ورقة عمل تلقائيًا

### ملاحظات

اسم الورقة التي تُضاف تلقائيًا (مثلًا بواسطة [`Add`](../../worksheetcollection/add/)) سيكون الاسم المحدد متبوعًا برقم تسلسلي. على سبيل المثال، قد يرغب مستخدم من ألمانيا أن يكون اسم الورقة "Tabellenblatt2" بدلاً من "Sheet2". ثم يمكن للمستخدم تنفيذ هذه الطريقة لإرجاع "Tabellenblatt".

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class GlobalizationSettingsMethodGetDefaultSheetNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // تعيين إعدادات العولمة المخصصة
            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                // احصل على اسم الورقة الافتراضي من إعدادات التعريب المخصصة
                string defaultSheetName = workbook.Settings.GlobalizationSettings.GetDefaultSheetName();
                Console.WriteLine($"Default sheet name retrieved: {defaultSheetName}");

                // إضافة ورقة عمل جديدة لتوضيح التسمية بناءً على الافتراضي المخصص
                int sheetIndex = workbook.Worksheets.Add();
                Worksheet newWorksheet = workbook.Worksheets[sheetIndex];
                Console.WriteLine($"New worksheet name after method call: {newWorksheet.Name}");

                Console.WriteLine("GetDefaultSheetName method demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDefaultSheetName method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("MethodGetDefaultSheetNameDemo.xlsx");
        }
    }

    // تنفيذ إعدادات التعريب المخصصة
    public class CustomGlobalizationSettings : GlobalizationSettings
    {
        public override string GetDefaultSheetName()
        {
            return "CustomSheet"; // Custom default sheet name
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


