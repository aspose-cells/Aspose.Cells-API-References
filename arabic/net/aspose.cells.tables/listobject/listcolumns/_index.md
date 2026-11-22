---
title: "ListObject.ListColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. يحصل على قائمة ListColumn لهذا الجدول"
type: docs
url: /ar/net/aspose.cells.tables/listobject/listcolumns/
---
## ListObject.ListColumns property

يحصل على قائمة [`ListColumn`](../../listcolumn/) لهذا الجدول.

```csharp
public ListColumnCollection ListColumns { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyListColumnsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // إنشاء كائن قائمة
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add(0, 0, 9, 4, true);
            ListObject listObject = listObjects[index];
            
            // تمكين الإجماليات وتعيين الحساب للعمود الخامس
            listObject.ShowTotals = true;
            listObject.ListColumns[4].TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Sum;
            
            // تطبيق نمط الجدول
            listObject.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleLight4;

            // احفظ المصنف
            workbook.Save("ListColumnsDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListColumnCollection](../../listcolumncollection/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


