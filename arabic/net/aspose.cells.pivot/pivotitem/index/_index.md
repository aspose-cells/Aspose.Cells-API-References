---
title: "PivotItem.Index"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotItem. تحصل على الفهرس الخاص بعنصر المحور في حقل الذاكرة المؤقتة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitem/index/
---
## PivotItem.Index property

يحصل على الفهرس الخاص بعنصر المحور في حقل الذاكرة المؤقتة.

```csharp
[Obsolete("Use PivotItem.Position property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Index { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن عُدِمت. بدلاً من ذلك، يرجى استخدام خاصية PivotItem.Position. سيتم إزالة هذه الطريقة بعد 6 أشهر منذ أغسطس 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemPropertyIndexDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;
            
            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // احصل على حقل الصف
            PivotField rowField = pivotTable.RowFields[0];
            
            // الوصول إلى عناصر المحور باستخدام خاصية Index
            foreach (PivotItem item in rowField.PivotItems)
            {
                Console.WriteLine($"Item: {item.Value}, Index: {item.Index}");
                
                // إخفاء تفاصيل العنصر باستخدام خاصية Index
                if (item.Value.ToString() == "Apple")
                {
                    rowField.HideItemDetail(item.Index, true);
                }
            }
            
            // احسب وقم بتحديث جدول المحور
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // احفظ المصنف
            workbook.Save("PivotItemPropertyIndexDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


