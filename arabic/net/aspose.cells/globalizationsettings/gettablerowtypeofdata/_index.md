---
title: "GlobalizationSettings.GetTableRowTypeOfData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة GlobalizationSettings. تحصل على اسم نوع صفوف الجدول التي تتكون من منطقة البيانات للجدول المشار إليه. الافتراضي هو Data لذا في الصيغة Data تمثل منطقة البيانات للجدول"
type: docs
url: /ar/net/aspose.cells/globalizationsettings/gettablerowtypeofdata/
---
## GlobalizationSettings.GetTableRowTypeOfData method

يحصل على اسم نوع صفوف الجدول التي تتكون من منطقة البيانات في الجدول المشار إليه. الافتراضي هو "Data"، لذا في الصيغة "#Data" تمثل منطقة البيانات للجدول.

```csharp
public virtual string GetTableRowTypeOfData()
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

    public class CustomGlobalizationSettings1 : GlobalizationSettings
    {
        public override string GetTableRowTypeOfData()
        {
            return "MyData";
        }
    }

    public class GlobalizationSettingsMethodGetTableRowTypeOfDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();

                worksheet.Cells["A1"].PutValue("Product");
                worksheet.Cells["B1"].PutValue("Price");
                worksheet.Cells["A2"].PutValue("Apple");
                worksheet.Cells["B2"].PutValue(2.5);
                worksheet.Cells["A3"].PutValue("Banana");
                worksheet.Cells["B3"].PutValue(1.8);

                // تم إصلاح معلمات ListObjects.Add لاستخدام التحميل الزائد الصحيح
                int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
                ListObject table = worksheet.ListObjects[tableIndex];
                table.ShowHeaderRow = true;
                table.DisplayName = "ProductTable";
                table.ShowTotals = true;
                table.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;

                Cell formulaCell = worksheet.Cells["B5"];
                formulaCell.Formula = "=SUM(ProductTable[#MyData])";

                workbook.CalculateFormula();
                Console.WriteLine($"Total price calculated: {formulaCell.Value}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTableRowTypeOfData method: {ex.Message}");
            }

            workbook.Save("MethodGetTableRowTypeOfDataDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


