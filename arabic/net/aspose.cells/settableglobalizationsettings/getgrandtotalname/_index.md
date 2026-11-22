---
title: "SettableGlobalizationSettings.GetGrandTotalName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SettableGlobalizationSettings. تحصل على اسم الإجمالي الكلي للدالة"
type: docs
url: /ar/net/aspose.cells/settableglobalizationsettings/getgrandtotalname/
---
## SettableGlobalizationSettings.GetGrandTotalName method

يحصل على اسم الإجمالي الكلي للدالة.

```csharp
public override string GetGrandTotalName(ConsolidationFunction functionType)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| functionType | ConsolidationFunction | نوع الدالة. |

### قيمة الإرجاع

اسم الإجمالي الكلي للدالة.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot; // Added this using directive
    using System;

    public class SettableGlobalizationSettingsMethodGetGrandTotalNameWithConsolidationFunctionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء إعدادات تعميم مخصصة
            SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
            
            // تعيين أسماء إجمالي كلي مخصصة لدوال التجميع المختلفة
            settings.SetGrandTotalName(ConsolidationFunction.Sum, "Custom Sum Grand Total");
            settings.SetGrandTotalName(ConsolidationFunction.Average, "Custom Average Grand Total");
            
            // طبق الإعدادات على المصنف
            workbook.Settings.GlobalizationSettings = settings;

            try
            {
                // استدعِ GetGrandTotalName مع دوال تجميع مختلفة
                string sumGrandTotalName = settings.GetGrandTotalName(ConsolidationFunction.Sum);
                string avgGrandTotalName = settings.GetGrandTotalName(ConsolidationFunction.Average);
                
                // أخرج النتائج
                Console.WriteLine("Sum Grand Total Name: " + sumGrandTotalName);
                Console.WriteLine("Average Grand Total Name: " + avgGrandTotalName);

                // إنشاء جدول محوري لتوضيح التأثير
                Cells cells = worksheet.Cells;
                cells["A1"].PutValue("Product");
                cells["B1"].PutValue("Sales");
                cells["A2"].PutValue("Apple");
                cells["B2"].PutValue(1000);
                cells["A3"].PutValue("Orange");
                cells["B3"].PutValue(2000);
                cells["A4"].PutValue("Banana");
                cells["B4"].PutValue(3000);

                PivotTableCollection pivotTables = worksheet.PivotTables;
                int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
                PivotTable pivotTable = pivotTables[index];
                pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[0].Function = ConsolidationFunction.Sum;
                
                // الطريقة الصحيحة لإضافة حقل بيانات آخر باستخدام دالة المتوسط
                pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
                pivotTable.DataFields[1].Function = ConsolidationFunction.Average;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetGrandTotalName method: {ex.Message}");
            }
            
            // احفظ المصنف
            workbook.Save("SettableGlobalizationSettingsMethodGetGrandTotalNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [ConsolidationFunction](../../consolidationfunction/)
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


