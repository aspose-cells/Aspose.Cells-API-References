---
title: "PivotTable.AddCalculatedField"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تضيف حقلًا محسوبًا إلى حقل المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/addcalculatedfield/
---
## AddCalculatedField(string, string, bool) {#addcalculatedfield_1}

يضيف حقلًا محسوبًا إلى حقل المحور.

```csharp
public void AddCalculatedField(string name, string formula, bool dragToDataArea)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الحقل المحسوب |
| صيغة | String | صيغة الحقل المحسوب. |
| dragToDataArea | منطقي | صحيح، اسحب هذا الحقل إلى منطقة البيانات فورًا |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddCalculatedFieldWithStringStringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "A";
            cells["B2"].Value = 100;
            cells["A3"].Value = "B";
            cells["B3"].Value = 150;
            cells["A4"].Value = "C";
            cells["B4"].Value = 200;

            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // إضافة حقل محسوب
            pivotTable.AddCalculatedField("DoubleSales", "=Sales*2", true);

            // احفظ المصنف
            workbook.Save("PivotTableWithCalculatedField.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddCalculatedField(string, string) {#addcalculatedfield}

يضيف حقلًا محسوبًا إلى حقل المحور ويسحبه إلى منطقة البيانات.

```csharp
public void AddCalculatedField(string name, string formula)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الحقل المحسوب |
| صيغة | String | صيغة الحقل المحسوب. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddCalculatedFieldWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);
            worksheet.Cells["B4"].PutValue(8);
            
            worksheet.Cells["C1"].PutValue("Quantity");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(3);
            worksheet.Cells["C4"].PutValue(10);

            // إنشاء مجموعة جداول محورية
            PivotTableCollection pivotTables = worksheet.PivotTables;
            
            // إضافة جدول محوري والحصول على فهرسه
            int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
            
            // الحصول على كائن جدول المحور
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // إضافة حقول إلى منطقة الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // إضافة حقول البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Price");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // إضافة حقل محسوب
            pivotTable.AddCalculatedField("Total", "=Price*Quantity");
            
            // تنسيق حقل البيانات
            pivotTable.DataFields["Total"].NumberFormat = "$#,##0.00";
            
            // تحديث وحساب الجدول المحوري
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // احفظ المصنف
            workbook.Save("PivotTableWithCalculatedField.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


