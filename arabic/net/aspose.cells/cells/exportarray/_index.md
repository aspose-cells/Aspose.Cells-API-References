---
title: "Cells.ExportArray"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تصدر البيانات في مجموعة Cells إلى كائن مصفوفة ثنائية الأبعاد"
type: docs
url: /ar/net/aspose.cells/cells/exportarray/
---
## Cells.ExportArray method

تصدير البيانات في مجموعة [`Cells`](../) إلى كائن مصفوفة ثنائية الأبعاد.

```csharp
public object[] ExportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم تصديرها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم تصديرها. |
| totalRows | Int32 | عدد الصفوف التي سيتم تصديرها |
| totalColumns | Int32 | عدد الأعمدة التي سيتم تصديرها |

### قيمة الإرجاع

كائن مصفوفة قيم الخلايا المصدرة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportArrayWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // املأ بعض بيانات العينة
            cells[0, 0].PutValue("A");
            cells[0, 1].PutValue("B");
            cells[1, 0].PutValue(10);
            cells[1, 1].PutValue(20);

            try
            {
                // تصدير البيانات إلى مصفوفة
                object[,] dataArray = cells.ExportArray(0, 0, 2, 2);
                
                // اعرض المصفوفة المصدرة
                for (int i = 0; i < 2; i++)
                {
                    for (int j = 0; j < 2; j++)
                    {
                        Console.Write(dataArray[i, j] + "\t");
                    }
                    Console.WriteLine();
                }
            }
            catch (CellsException ex)
            {
                Console.WriteLine("Error exporting array: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


