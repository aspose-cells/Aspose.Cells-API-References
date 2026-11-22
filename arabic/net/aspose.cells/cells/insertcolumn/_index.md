---
title: "Cells.InsertColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تُدرج عمودًا جديدًا في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/cells/insertcolumn/
---
## InsertColumn(int, bool) {#insertcolumn_1}

يدرج عمودًا جديدًا في ورقة العمل.

```csharp
public void InsertColumn(int columnIndex, bool updateReference)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود. |
| updateReference | منطقي | يشير إلى ما إذا كانت المراجع في أوراق عمل أخرى سيتم تحديثها. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // املأ بعض البيانات النموذجية في العمود 0
            Cells cells = sheet.Cells;
            for (int i = 0; i < 5; i++)
            {
                cells[i, 0].PutValue($"Original {i}");
            }

            // أدرج عمودًا جديدًا عند الفهرس 1 وحرك الأعمدة إلى اليمين
            cells.InsertColumn(1, true);

            // انسخ البيانات من العمود 0 إلى العمود الجديد 1
            cells.CopyColumn(cells, 0, 1);

            // احفظ المصنف
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumn(int) {#insertcolumn}

يدرج عمودًا جديدًا في ورقة العمل.

```csharp
public void InsertColumn(int columnIndex)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnWithInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheet = workbook.Worksheets[0];
            
            // احصل على مجموعة الخلايا
            Cells cells = sheet.Cells;
            
            // أدرج بيانات في الخلايا للعرض
            cells["A1"].PutValue("Column A");
            cells["B1"].PutValue("Column B");
            cells["C1"].PutValue("Column C");
            
            // أدرج عمودًا جديدًا عند الفهرس 1 (سيصبح العمود الجديد B)
            cells.InsertColumn(1);
            
            // تحقق عن طريق إدراج بيانات في العمود الجديد
            cells["B1"].PutValue("New Column");
            
            // احفظ المصنف
            workbook.Save("InsertColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


