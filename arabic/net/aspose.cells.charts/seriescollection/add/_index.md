---
title: "SeriesCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SeriesCollection. تضيف مجموعة Series إلى مخطط"
type: docs
url: /ar/net/aspose.cells.charts/seriescollection/add/
---
## Add(string, bool) {#add}

تضيف مجموعة [`Series`](../../series/) إلى مخطط.

```csharp
public int Add(string dataArea, bool isVertical)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| dataArea | String | يحدد القيم التي سيتم رسم سلسلة البيانات منها |
| isVertical | Boolean | يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. إذا كان صحيحًا، سيتم إضافة [`Series`](../../series/) عمودًا بعمود. |

### قيمة الإرجاع

إرجاع الفهرس الأول للسلسلة ASeries المضافة في NSeries.

### ملاحظات

إذا تم تعيين البيانات على خلايا متجاورة، استخدم النقطتين للفصل بينها. على سبيل المثال، $C$2:$C$5. إذا تم تعيين البيانات على خلايا غير متجاورة، استخدم الفاصلة للفصل بينها. على سبيل المثال: ($C$2,$D$5). هذه الطريقة تعالج ببساطة *dataArea* كنطاق بيانات. إذا كنت تريد فحص طريقة ChartCollection.Add() بذكاء.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddWithStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B4"].PutValue(30);

            // إنشاء مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // أضف سلسلة باستخدام معلمات نصية ومنطقية
            chart.NSeries.Add("=Sheet1!A1:B4", true);
            
            // احفظ المصنف
            workbook.Save("SeriesCollectionMethodAddWithStringBooleanDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, bool, bool) {#add_1}

تضيف مجموعة [`Series`](../../series/) إلى مخطط.

```csharp
public int Add(string area, bool isVertical, bool checkLabels)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| منطقة | String | يحدد القيم التي سيتم رسم سلسلة البيانات منها |
| isVertical | منطقي | يحدد ما إذا كان سيتم رسم السلسلة من نطاق قيم الخلايا حسب الصف أو حسب العمود. |
| checkLabels | منطقي | يشير إلى ما إذا كان النطاق يحتوي على اسم السلسلة |

### قيمة الإرجاع

إرجاع الفهرس الأول للسلسلة ASeries المضافة في NSeries.

### ملاحظات

إذا تم تعيين البيانات على خلايا متجاورة، استخدم النقطتين للفصل بينها. على سبيل المثال، $C$2:$C$5. إذا تم تعيين البيانات على خلايا غير متجاورة، استخدم الفاصلة للفصل بينها. على سبيل المثال، ($C$2,$D$5).

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionMethodAddWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("Category1");
            sheet.Cells["A2"].PutValue(10);
            sheet.Cells["A3"].PutValue(20);
            sheet.Cells["B1"].PutValue("Category2");
            sheet.Cells["B2"].PutValue(30);
            sheet.Cells["B3"].PutValue(40);

            // إنشاء مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // أضف سلسلة باستخدام طريقة Add مع معلمات نصية ومنطقية
            chart.NSeries.Add("=Sheet1!$B$2:$B$3", true, false);
            chart.NSeries.CategoryData = "=Sheet1!$A$1:$B$1";
            
            // احفظ المصنف
            wb.Save("SeriesCollectionMethodAddWithStringBooleanBooleanDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


