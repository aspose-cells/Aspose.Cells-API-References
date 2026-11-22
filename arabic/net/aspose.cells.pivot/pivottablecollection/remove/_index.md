---
title: "PivotTableCollection.Remove"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTableCollection. تحذف جدول PivotTable المحدد وتحذف بيانات جدول PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivottablecollection/remove/
---
## Remove(PivotTable) {#remove}

يحذف PivotTable المحدد ويحذف بيانات PivotTable

```csharp
public void Remove(PivotTable pivotTable)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotTable | PivotTable | كائن PivotTable |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("PivotTableExample.xlsx");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // الحصول على مجموعة الجداول المحورية
            PivotTableCollection pivotTables = sheet.PivotTables;
            
            // تحقق مما إذا كان هناك أي جداول محور
            if (pivotTables.Count > 0)
            {
                // احصل على أول جدول محور
                PivotTable pivotTable = pivotTables[0];
                
                // إزالة جدول PivotTable
                pivotTables.Remove(pivotTable);
                
                Console.WriteLine("Pivot table removed successfully. Count: " + pivotTables.Count);
            }
            
            // احفظ المصنف
            workbook.Save("PivotTableRemoved.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Remove(PivotTable, bool) {#remove_1}

يحذف PivotTable المحدد

```csharp
public void Remove(PivotTable pivotTable, bool keepData)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotTable | PivotTable | كائن PivotTable |
| keepData | منطقي | ما إذا كان يجب الاحتفاظ ببيانات PivotTable |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCollectionMethodRemoveWithPivotTableBooleanDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // إضافة جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "D5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // عرض طريقة Remove مع PivotTable ومعلمات منطقية
            Console.WriteLine("Before removal - Cell D5 value: " + worksheet.Cells["D5"].StringValue);
            
            // إزالة جدول PivotTable مع الحفاظ على البيانات (true)
            worksheet.PivotTables.Remove(pivotTable, true);
            Console.WriteLine("After removal (keep data) - Cell D5 value: " + worksheet.Cells["D5"].StringValue);

            // إضافة جدول محوري آخر
            index = worksheet.PivotTables.Add("A1:B4", "D10", "PivotTable2");
            pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            Console.WriteLine("\nBefore removal - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
            
            // إزالة جدول PivotTable ومسح البيانات (false)
            worksheet.PivotTables.Remove(pivotTable, false);
            Console.WriteLine("After removal (clear data) - Cell D10 value: " + worksheet.Cells["D10"].StringValue);
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../../pivottable/)
* class [PivotTableCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


