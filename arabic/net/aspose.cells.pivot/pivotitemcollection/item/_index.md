---
title: "PivotItemCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "PivotItemCollection property. تحصل على كائن PivotItem في الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells.pivot/pivotitemcollection/item/
---
## PivotItemCollection indexer (1 of 2)

تحصل على كائن PivotItem في الفهرس المحدد.

```csharp
public PivotItem this[int index] { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 150;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 200;
            
            // إنشاء جدول محوري
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // الوصول إلى عناصر المحور باستخدام خاصية Item
            PivotItemCollection pivotItems = pivotTable.RowFields[0].PivotItems;
            
            // عرض استخدام خاصية Item
            Console.WriteLine("First pivot item: " + pivotItems[0].Name);
            Console.WriteLine("Second pivot item: " + pivotItems[1].Name);
            Console.WriteLine("Third pivot item: " + pivotItems[2].Name);
        }
    }
}
```

### انظر أيضًا

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## PivotItemCollection indexer (2 of 2)

تحصل على [`PivotItem`](../../pivotitem/) بالاسم المحدد.

```csharp
public PivotItem this[string itemValue] { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotItemCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("PivotTest3.xlsx");
            
            // أضف ورقة عمل جديدة للجدول المحوري
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            Worksheet dataSheet = workbook.Worksheets["New Hardware - Yearly"];

            // إضافة جدول محوري
            PivotTableCollection pivotTables = pivotSheet.PivotTables;
            int index = pivotTables.Add("='New Hardware - Yearly'!A1:D621", "A3", "PivotTable");
            PivotTable pivotTable = pivotTables[index];

            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "2014");

            // تكوين جدول محوري
            pivotTable.RowFields["Vendor"].SetSubtotals(PivotFieldSubtotalType.None, true);
            pivotTable.ShowColumnGrandTotals = false;

            // تحديث وحساب البيانات
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // عرض استخدام خاصية Item وعمليات النقل
            PivotItemCollection items = pivotTable.RowFields["Item"].PivotItems;
            
            // الوصول إلى العناصر باستخدام خاصية Item
            items["4H12"].Move(0, true);
            items["DIF400"].Move(-1, true);
            
            pivotTable.CalculateData();
            
            items["CA32"].Move(0, true);
            items["AAA3"].Move(-1, true);

            // احفظ المصنف
            workbook.Save("PivotItemCollectionDemo_Output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotItem](../../pivotitem/)
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


