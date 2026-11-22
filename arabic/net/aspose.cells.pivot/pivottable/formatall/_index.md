---
title: "PivotTable.FormatAll"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تنسيق جميع الخلايا في منطقة جدول المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/formatall/
---
## PivotTable.FormatAll method

تنسيق جميع الخلايا في منطقة جدول المحور

```csharp
public void FormatAll(Style style)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| النمط | النمط | النمط الذي سيتم تنسيقه |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatAllWithStyleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            var cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;
            
            // إنشاء جدول محوري
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // إضافة حقول إلى جدول محوري
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // إنشاء وتكوين النمط
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;
            
            // تطبيق النمط على جدول المحور بالكامل
            pivotTable.FormatAll(style);
            
            // احفظ المصنف
            workbook.Save("PivotTableFormatAllDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


