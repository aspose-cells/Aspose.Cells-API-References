---
title: "PivotTable.Format"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تقوم بتنسيق المنطقة المحددة من PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/format/
---
## Format(PivotArea, Style) {#format_1}

يقوم بتنسيق المنطقة المحددة في جدول المحور.

```csharp
public void Format(PivotArea pivotArea, Style style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotArea | PivotArea | منطقة عرض Pivot المحددة. |
| النمط | النمط | الإعداد المُنسق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotTableMethodFormatWithPivotAreaStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للجدول المحوري
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["A4"].Value = "Truck";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 5000;
            worksheet.Cells["B3"].Value = 12000;
            worksheet.Cells["B4"].Value = 8000;

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D3", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى الجدول المحوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // احسب البيانات لملء جدول المحور
            pivotTable.CalculateData();

            // إنشاء نمط للتنسيق
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // إنشاء منطقة Pivot للتنسيق
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.AxisType = PivotFieldType.Data;

            try
            {
                // تطبيق التنسيق على منطقة Pivot
                pivotTable.Format(pivotArea, style);
                
                Console.WriteLine("Format method executed successfully with parameters (PivotArea, Style)");
                
                // احفظ المصنف لإظهار التأثير
                workbook.Save("PivotTableFormatWithPivotAreaStyleDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Format method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [PivotArea](../../pivotarea/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Format(CellArea, Style) {#format}

يقوم بتنسيق المنطقة المحددة في جدول المحور.

```csharp
public void Format(CellArea ca, Style style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | CellArea | نطاق الخلايا. |
| النمط | النمط | النمط |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;
    using System.Drawing;

    public class PivotTableMethodFormatWithCellAreaStyleDemo
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
            worksheet.Cells["C3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Product C");
            worksheet.Cells["B4"].PutValue("East");
            worksheet.Cells["C4"].PutValue(3000);

            // إنشاء جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة صفوف وحقول بيانات
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // حساب البيانات والنطاقات
            pivotTable.CalculateData();
            pivotTable.CalculateRange();

            // إنشاء نمط للتنسيق
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;
            style.ForegroundColor = Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // تحديد منطقة الخلية للتنسيق (نطاق جسم البيانات)
            CellArea area = pivotTable.DataBodyRange;

            try
            {
                // استدعاء طريقة Format مع معلمات CellArea و Style
                pivotTable.Format(area, style);
                
                Console.WriteLine("PivotTable formatted successfully with parameters (CellArea, Style)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error formatting PivotTable: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("PivotTableFormatWithCellAreaStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)

---

## Format(int, int, Style) {#format_2}

يقوم بتنسيق الخلية في منطقة جدول المحور

```csharp
public void Format(int row, int column, Style style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف للخلية |
| عمود | Int32 | فهرس العمود للخلية |
| النمط | النمط | النمط الذي يُستخدم لتنسيق الخلية |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatWithInt32Int32StyleDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);

            // إضافة جدول محوري
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // إضافة حقول إلى منطقة الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // حساب البيانات
            pivotTable.CalculateData();

            // إنشاء نمط للتنسيق
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.LightBlue;
            style.Font.IsBold = true;

            // تنسيق خلية رأس جدول محوري (الصف 2، العمود 0 في إحداثيات جدول محوري)
            pivotTable.Format(2, 0, style);

            // احفظ المصنف
            workbook.Save("PivotTableFormatDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


