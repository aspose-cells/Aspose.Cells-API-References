---
title: "PivotTable.AddFieldToArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تضيف الحقل إلى المنطقة المحددة"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/addfieldtoarea/
---
## AddFieldToArea(PivotFieldType, string) {#addfieldtoarea_2}

يضيف الحقل إلى المنطقة المحددة.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, string fieldName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | PivotFieldType | نوع منطقة الحقول. |
| fieldName | String | الاسم في الحقول الأساسية. |

### قيمة الإرجاع

موضع الحقل في الحقول المحددة. إذا لم يكن هناك حقل يحمل هذا الاسم، أعد -1.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypeStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            cells["A2"].Value = "P1";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            cells["A3"].Value = "P2";
            cells["B3"].Value = "South";
            cells["C3"].Value = 1500;
            cells["A4"].Value = "P3";
            cells["B4"].Value = "East";
            cells["C4"].Value = 2000;
            cells["A5"].Value = "P1";
            cells["B5"].Value = "West";
            cells["C5"].Value = 1200;

            // إضافة جدول محوري
            int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[index];

            // إضافة حقول إلى مناطق مختلفة باستخدام AddFieldToArea مع أسماء الحقول كسلاسل نصية
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Column, "Region");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // تحديث وحساب الجدول المحوري
            pivot.RefreshData();
            pivot.CalculateData();

            // احفظ المصنف
            workbook.Save("PivotTableDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldToArea(PivotFieldType, int) {#addfieldtoarea_1}

يضيف الحقل إلى المنطقة المحددة.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, int baseFieldIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | PivotFieldType | نوع منطقة الحقول. |
| baseFieldIndex | Int32 | الفهرس في الحقول الأساسية. |

### قيمة الإرجاع

موضع الحقل في الحقول المحددة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypeInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى PivotTable
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Region");
            worksheet.Cells["C1"].PutValue("Sales");
            
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Product " + (i % 3 + 1));
                worksheet.Cells["B" + i].PutValue("Region " + (i % 2 + 1));
                worksheet.Cells["C" + i].PutValue(i * 100);
            }

            // إضافة PivotTable
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // إضافة حقول إلى المناطق باستخدام AddFieldToArea(PivotFieldType, Int32)
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row field
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column field
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data field

            // احفظ المصنف
            workbook.Save("PivotTableDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## AddFieldToArea(PivotFieldType, PivotField) {#addfieldtoarea}

يضيف الحقل إلى المنطقة المحددة.

```csharp
public int AddFieldToArea(PivotFieldType fieldType, PivotField pivotField)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldType | PivotFieldType | نوع منطقة الحقول. |
| pivotField | PivotField | الحقل في الحقول الأساسية. |

### قيمة الإرجاع

موضع الحقل في الحقول المحددة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodAddFieldToAreaWithPivotFieldTypePivotFieldDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل ببيانات المصدر
            Worksheet sourceSheet = workbook.Worksheets[0];
            sourceSheet.Name = "Source Data";
            
            // أضف بيانات تجريبية
            sourceSheet.Cells["A1"].PutValue("Product");
            sourceSheet.Cells["B1"].PutValue("Region");
            sourceSheet.Cells["C1"].PutValue("Sales");
            
            sourceSheet.Cells["A2"].PutValue("Product A");
            sourceSheet.Cells["B2"].PutValue("North");
            sourceSheet.Cells["C2"].PutValue(1000);
            
            sourceSheet.Cells["A3"].PutValue("Product B");
            sourceSheet.Cells["B3"].PutValue("South");
            sourceSheet.Cells["C3"].PutValue(2000);
            
            sourceSheet.Cells["A4"].PutValue("Product A");
            sourceSheet.Cells["B4"].PutValue("East");
            sourceSheet.Cells["C4"].PutValue(1500);
            
            sourceSheet.Cells["A5"].PutValue("Product B");
            sourceSheet.Cells["B5"].PutValue("West");
            sourceSheet.Cells["C5"].PutValue(2500);

            // إضافة جدول محوري
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            string source = "='Source Data'!A1:C5";
            int index = pivotTables.Add(source, "A1", "PivotTable");
            PivotTable pTable = pivotTables[index];

            // إضافة حقول إلى المناطق
            pTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pTable.AddFieldToArea(PivotFieldType.Row, 1); // Region
            
            // إضافة حقل البيانات
            pTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pTable.DataFields[0].Function = ConsolidationFunction.Sum;
            pTable.DataFields[0].NumberFormat = "$0.00";

            // إضافة حقل بيانات إلى منطقة الأعمدة باستخدام معلمة PivotField
            if (pTable.DataField != null)
            {
                pTable.AddFieldToArea(PivotFieldType.Column, pTable.DataField);
            }

            // احفظ المصنف
            workbook.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


