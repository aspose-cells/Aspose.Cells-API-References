---
title: "PivotAreaCollection.RemoveAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotAreaCollection. إزالة إعداد منطقة محورية مشروطة منسقة واحدة"
type: docs
url: /ar/net/aspose.cells.pivot/pivotareacollection/removeat/
---
## PivotAreaCollection.RemoveAt method

إزالة إعداد منطقة محورية مشروطة منسقة واحدة.

```csharp
public void RemoveAt(int index)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | الفهرس |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotAreaCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء بيانات عينة لجدول محوري
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // إضافة جدول محوري
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];

            // حدد مناطق خلايا لإضافتها إلى مناطق المحور
            CellArea cellArea1 = new CellArea();
            cellArea1.StartRow = 0;
            cellArea1.StartColumn = 0;
            cellArea1.EndRow = 2;
            cellArea1.EndColumn = 1;

            CellArea cellArea2 = new CellArea();
            cellArea2.StartRow = 1;
            cellArea2.StartColumn = 1;
            cellArea2.EndRow = 3;
            cellArea2.EndColumn = 2;

            // احصل على مجموعة مناطق المحور عن طريق تحديد المنطقة
            PivotAreaCollection pivotAreas = pivotTable.SelectArea(cellArea1);
            pivotAreas.Add(cellArea2);

            try
            {
                // اعرض مناطق المحور قبل الإزالة
                Console.WriteLine("Pivot areas before removal:");
                for (int i = 0; i < pivotAreas.Count; i++)
                {
                    CellArea[] areas = pivotAreas[i].GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Area {i}: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }

                // استدعِ طريقة RemoveAt مع معامل Int32
                pivotAreas.RemoveAt(0);

                Console.WriteLine("\nPivot areas after removal:");
                for (int i = 0; i < pivotAreas.Count; i++)
                {
                    CellArea[] areas = pivotAreas[i].GetCellAreas();
                    foreach (CellArea ca in areas)
                    {
                        Console.WriteLine($"Area {i}: ({ca.StartRow},{ca.StartColumn}) to ({ca.EndRow},{ca.EndColumn})");
                    }
                }
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // حفظ النتيجة
            workbook.Save("PivotAreaCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotAreaCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


