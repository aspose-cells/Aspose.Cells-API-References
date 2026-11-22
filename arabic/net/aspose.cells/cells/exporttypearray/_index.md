---
title: "Cells.ExportTypeArray"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تصدر نوع قيمة الخلية في مجموعة Cells إلى كائن مصفوفة ثنائية الأبعاد"
type: docs
url: /ar/net/aspose.cells/cells/exporttypearray/
---
## Cells.ExportTypeArray method

تصدير نوع قيمة الخلية في مجموعة [`Cells`](../) إلى كائن مصفوفة ثنائية الأبعاد.

```csharp
public CellValueType[] ExportTypeArray(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم تصديرها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم تصديرها. |
| totalRows | Int32 | عدد الصفوف التي سيتم تصديرها. |
| totalColumns | Int32 | عدد الأعمدة التي سيتم تصديرها. |

### قيمة الإرجاع

كائن المصفوفة المُصدَّر الذي يمثل أنواع قيم الخلايا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportTypeArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين القيم في الخلايا
            cells["A1"].PutValue(10);
            cells["B1"].PutValue("Hello");
            cells["A2"].PutValue(true);
            cells["B2"].PutValue(DateTime.Now);

            // تصدير أنواع الخلايا إلى مصفوفة ثنائية الأبعاد
            CellValueType[,] typeArray = cells.ExportTypeArray(0, 0, 2, 2);

            // عرض النتائج
            for (int i = 0; i < 2; i++)
            {
                for (int j = 0; j < 2; j++)
                {
                    Console.WriteLine($"Cell[{i},{j}] Type: {typeArray[i, j]}");
                }
            }

            // إظهار حالة الاستثناء
            try
            {
                CellValueType[,] invalidArray = cells.ExportTypeArray(-1, 0, 2, 2);
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Exception caught as expected: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* enum [CellValueType](../../cellvaluetype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


