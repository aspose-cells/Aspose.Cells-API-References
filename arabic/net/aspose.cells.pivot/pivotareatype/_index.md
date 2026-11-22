---
title: "تعداد PivotAreaType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Pivot.PivotAreaType. يشير إلى نوع القاعدة المستخدمة لوصف منطقة أو جانب من PivotTable"
type: docs
url: /ar/net/aspose.cells.pivot/pivotareatype/
---
## PivotAreaType enumeration

يشير إلى نوع القاعدة المستخدمة لوصف منطقة أو جانب من جدول محوري.

```csharp
public enum PivotAreaType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | لا توجد منطقة Pivot. |
| Normal | `1` | يمثل عنوانًا أو عنصرًا. |
| Data | `2` | يمثل شيئًا في منطقة البيانات. |
| All | `3` | يمثل PivotTable بالكامل. |
| Origin | `4` | يمثل الخلايا الفارغة في أعلى اليسار من PivotTable (أعلى اليمين للأوراق RTL). |
| Button | `5` | يمثل زر الحقل. |
| TopRight | `6` | يمثل الخلايا الفارغة في أعلى اليمين من PivotTable (أعلى اليسار للأوراق RTL). |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaTypeDemo
    {
        public static void PivotAreaTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["A4"].PutValue("Bananas");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);

            // إنشاء PivotTable
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // إضافة حقول إلى PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // إنشاء PivotArea لـ PivotTable
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true;
            pivotArea.IsRowGrandIncluded = true;

            // إخراج خصائص PivotArea
            Console.WriteLine("Pivot Area Type: " + pivotArea.RuleType);
            Console.WriteLine("Only Data: " + pivotArea.OnlyData);
            Console.WriteLine("Is Row Grand Included: " + pivotArea.IsRowGrandIncluded);

            // احفظ المصنف
            workbook.Save("PivotAreaTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


