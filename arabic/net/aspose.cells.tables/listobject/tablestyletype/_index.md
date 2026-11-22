---
title: "ListObject.TableStyleType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ListObject. يحصل على نمط الجدول المدمج"
type: docs
url: /ar/net/aspose.cells.tables/listobject/tablestyletype/
---
## ListObject.TableStyleType property

يحصل على النمط المدمج للجدول.

```csharp
public TableStyleType TableStyleType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyTableStyleTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية إلى الخلايا
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i+1}-{j+1}");
                }
            }
            
            // احصل على مجموعة كائنات القائمة
            ListObjectCollection tables = worksheet.ListObjects;
            
            // إضافة جدول
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[0];
            
            // تعيين نمط الجدول
            table.TableStyleType = TableStyleType.TableStyleDark2;
            
            // احفظ المصنف
            workbook.Save("TableStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TableStyleType](../../tablestyletype/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


