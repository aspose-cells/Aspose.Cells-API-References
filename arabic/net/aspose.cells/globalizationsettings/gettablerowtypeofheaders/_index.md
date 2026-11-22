---
title: "GlobalizationSettings.GetTableRowTypeOfHeaders"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. يحصل على اسم نوع صفوف الجدول التي تتكون من رأس الجدول. الافتراضي هو Headers لذا في الصيغة يمثل Headers رأس الجدول"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/gettablerowtypeofheaders/
---
## GlobalizationSettings.GetTableRowTypeOfHeaders method

يحصل على اسم نوع صفوف الجدول التي تتكون من رأس الجدول. الافتراضي هو "Headers"، لذا في الصيغة "#Headers" تمثل رأس الجدول.

```csharp
public virtual string GetTableRowTypeOfHeaders()
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

    public class GlobalizationSettingsMethodGetTableRowTypeOfHeadersDemo
    {
        public class CustomGlobalizationSettings : GlobalizationSettings
        {
            public override string GetTableRowTypeOfHeaders()
            {
                return "MyHeaders";
            }
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["B1"].Value = "Price";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["B2"].Value = 2.5;
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["B3"].Value = 1.8;

            // تم إصلاح إنشاء ListObject عن طريق معالجة قيمة الإرجاع من Add()
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            // استخدم الخاصية DisplayName بدلاً من Name
            table.DisplayName = "FruitTable";

            workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

            try
            {
                worksheet.Cells["A5"].Formula = "=COUNTA(FruitTable[#MyHeaders])";
                workbook.CalculateFormula();
                Console.WriteLine("Method executed successfully. Header count: " + worksheet.Cells["A5"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfHeaders method: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfHeadersDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


