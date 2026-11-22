---
title: "PivotTable.ValuesField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotTable. تحصل على كائن PivotField يمثل جميع حقول البيانات في جدول البيفوت. للقراءة فقط. يتم إنشاؤه فقط عندما يكون هناك حقلان بيانات أو أكثر في منطقة البيانات. بشكل افتراضي يكون في منطقة الصف. يمكنك سحبه إلى منطقة الصف/العمود باستخدام طريقة PivotTable.AddFieldToArea."
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/valuesfield/
---
## PivotTable.ValuesField property

يحصل على كائن [`PivotField`](../../pivotfield/) يمثل جميع حقول البيانات في جدول البيفوت. للقراءة فقط. يتم إنشاؤه فقط عندما يكون هناك حقلان بيانات أو أكثر في منطقة البيانات. بشكل افتراضي يكون في منطقة الصف. يمكنك سحبه إلى منطقة الصف/العمود باستخدام طريقة PivotTable.AddFieldToArea() .

```csharp
public PivotField ValuesField { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTablePropertyValuesFieldDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue("North");
            worksheet.Cells["C2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B3"].PutValue("South");
            worksheet.Cells["C3"].PutValue(1500);
            worksheet.Cells["A4"].PutValue("Product A");
            worksheet.Cells["B4"].PutValue("South");
            worksheet.Cells["C4"].PutValue(2000);
            worksheet.Cells["A5"].PutValue("Product B");
            worksheet.Cells["B5"].PutValue("North");
            worksheet.Cells["C5"].PutValue(1200);

            try
            {
                // إنشاء جدول محوري
                int pivotIndex = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
                PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

                // إضافة حقول إلى المناطق
                pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
                pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
                pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

                // احسب البيانات لملء جدول المحور
                pivotTable.CalculateData();

                // الوصول إلى خاصية ValuesField (للقراءة فقط)
                PivotField valuesField = pivotTable.ValuesField;

                if (valuesField != null)
                {
                    Console.WriteLine("ValuesField Name: " + valuesField.Name);
                    Console.WriteLine("ValuesField DisplayName: " + valuesField.DisplayName);
                    Console.WriteLine("ValuesField Position: " + valuesField.Position);
                    Console.WriteLine("ValuesField RegionType: " + valuesField.RegionType);
                    Console.WriteLine("ValuesField IsValuesField: " + valuesField.IsValuesField);
                }
                else
                {
                    Console.WriteLine("ValuesField is null - no data fields in the pivot table");
                }

                // احفظ المصنف
                workbook.Save("PivotTableValuesFieldDemo.xlsx");
                Console.WriteLine("PivotTable with ValuesField demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


