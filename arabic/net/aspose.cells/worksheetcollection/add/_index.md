---
title: "WorksheetCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة WorksheetCollection. تضيف ورقة عمل إلى المجموعة"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/add/
---
## Add(SheetType) {#add_2}

يضيف ورقة عمل إلى المجموعة.

```csharp
public int Add(SheetType type)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| type | SheetType | نوع Worksheet. |

### قيمة الإرجاع

[`Worksheet`](../../worksheet/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddWithSheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // إضافة ورقة مخطط جديدة باستخدام معلمة SheetType
            workbook.Worksheets.Add(SheetType.Chart);
            
            // إضافة بيانات إلى ورقة العمل الأولى
            Cells cells = workbook.Worksheets[0].Cells;
            cells["C2"].PutValue(5000);
            cells["C3"].PutValue(3000);
            cells["C4"].PutValue(4000);
            cells["C5"].PutValue(5000);
            cells["C6"].PutValue(6000);
            
            // إنشاء مخطط في ورقة المخطط
            Aspose.Cells.Charts.ChartCollection charts = workbook.Worksheets[1].Charts;
            int chartIndex = charts.Add(Aspose.Cells.Charts.ChartType.Column, 10, 10, 20, 20);
            Aspose.Cells.Charts.Chart chart = charts[chartIndex];
            chart.NSeries.Add("Sheet1!C2:C6", true);
            
            // احفظ دفتر العمل (اختياري)
            // workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add() {#add_1}

يضيف ورقة عمل إلى المجموعة.

```csharp
public int Add()
```

### قيمة الإرجاع

[`Worksheet`](../../worksheet/) object index.

### انظر أيضًا

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add}

يضيف ورقة عمل إلى المجموعة.

```csharp
public Worksheet Add(string sheetName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | String | اسم Worksheet |

### قيمة الإرجاع

[`Worksheet`](../../worksheet/) object.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets.Add("NewSheet");
            
            // إضافة بيانات إلى ورقة العمل الجديدة
            worksheet.Cells["A1"].PutValue("Worksheet added successfully!");
            
            // احفظ المصنف
            wb.Save("WorksheetCollectionMethodAddWithStringDemo_output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


