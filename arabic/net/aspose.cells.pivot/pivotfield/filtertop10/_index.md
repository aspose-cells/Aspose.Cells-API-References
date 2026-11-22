---
title: "PivotField.FilterTop10"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. تقوم بتصفية القيم لحقل البيانات المحوري"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/filtertop10/
---
## PivotField.FilterTop10 method

تصفية حسب القيم لحقل pivot للبيانات.

```csharp
public PivotFilter FilterTop10(int valueFieldIndex, PivotFilterType type, bool isTop, int itemCount)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| valueFieldIndex | Int32 | فهرس حقل البيانات في منطقة البيانات. |
| type | PivotFilterType | نوع تصفية البيانات. يمكن أن يكون فقط Count أو Sum أو Percent. |
| isTop | منطقي | يشير إلى ما إذا كان الفلتر من الأعلى أم من الأسفل |
| itemCount | Int32 | عدد العناصر |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodFilterTop10WithInt32PivotFilterTypeBooleanIntDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لجدول محوري
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["A5"].Value = "Apple";
            worksheet.Cells["A6"].Value = "Orange";
            worksheet.Cells["A7"].Value = "Banana";
            worksheet.Cells["A8"].Value = "Apple";
            
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["B4"].Value = 30;
            worksheet.Cells["B5"].Value = 40;
            worksheet.Cells["B6"].Value = 50;
            worksheet.Cells["B7"].Value = 60;
            worksheet.Cells["B8"].Value = 70;

            // إنشاء جدول محوري
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B8", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // إضافة حقل الصف
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // إضافة حقل البيانات
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // تطبيق فلتر أعلى 10
            pivotTable.BaseFields[0].FilterTop10(0, PivotFilterType.Count, false, 2);
            
            // احفظ المصنف
            workbook.Save("PivotTableFilterTop10.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


