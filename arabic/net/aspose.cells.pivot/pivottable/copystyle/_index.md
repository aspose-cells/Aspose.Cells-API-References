---
title: "PivotTable.CopyStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotTable. تنسخ النمط المسمى من جدول محوري آخر"
type: docs
url: /ar/net/aspose.cells.pivot/pivottable/copystyle/
---
## PivotTable.CopyStyle method

ينسخ النمط المسمى من جدول محور آخر.

```csharp
public void CopyStyle(PivotTable pivotTable)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| pivotTable | PivotTable | جدول محوري المصدر. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCopyStyleWithPivotTableDemo
    {
        public static void Run()
        {
            // إنشاء مصنف المصدر مع جدول محوري
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            sourceSheet.Cells["A1"].PutValue("Product");
            sourceSheet.Cells["B1"].PutValue("Sales");
            sourceSheet.Cells["A2"].PutValue("A");
            sourceSheet.Cells["B2"].PutValue(100);
            sourceSheet.Cells["A3"].PutValue("B");
            sourceSheet.Cells["B3"].PutValue(200);
            
            // إنشاء جدول محوري المصدر (احصل صراحةً على كائن الجدول المحوري)
            PivotTable sourcePivotTable = sourceSheet.PivotTables[sourceSheet.PivotTables.Add("PivotTable1", "A1:B3", "C3")];
            sourcePivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            sourcePivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // تطبيق النمط على جدول محوري المصدر
            sourcePivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
            
            // إنشاء مصنف الوجهة مع جدول محوري
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];
            
            // إضافة نفس بنية البيانات
            destSheet.Cells["A1"].PutValue("Product");
            destSheet.Cells["B1"].PutValue("Sales");
            destSheet.Cells["A2"].PutValue("A");
            destSheet.Cells["B2"].PutValue(150);
            destSheet.Cells["A3"].PutValue("B");
            destSheet.Cells["B3"].PutValue(250);
            
            // إنشاء جدول محوري الوجهة (احصل صراحةً على كائن الجدول المحوري)
            PivotTable destPivotTable = destSheet.PivotTables[destSheet.PivotTables.Add("PivotTable2", "A1:B3", "C3")];
            destPivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            destPivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // نسخ النمط من المصدر إلى جدول محوري الوجهة
            destPivotTable.CopyStyle(sourcePivotTable);
            
            // حفظ النتيجة
            destWorkbook.Save("PivotTableStyleCopied.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


