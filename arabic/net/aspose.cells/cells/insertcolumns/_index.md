---
title: "Cells.InsertColumns"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تُدرج بعض الأعمدة في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/cells/insertcolumns/
---
## InsertColumns(int, int) {#insertcolumns}

يدرج بعض الأعمدة في ورقة العمل.

```csharp
public void InsertColumns(int columnIndex, int totalColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود. |
| totalColumns | Int32 | عدد الأعمدة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إدراج 3 أعمدة بدءًا من فهرس العمود 1 (العمود الثاني)
            worksheet.Cells.InsertColumns(1, 3);
            
            // أضف بيانات عينة لتوضيح الأعمدة المُدرجة
            worksheet.Cells["A1"].PutValue("Original Column");
            worksheet.Cells["B1"].PutValue("Inserted Column 1");
            worksheet.Cells["C1"].PutValue("Inserted Column 2");
            worksheet.Cells["D1"].PutValue("Inserted Column 3");
            worksheet.Cells["E1"].PutValue("Original Column 2");
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, bool) {#insertcolumns_2}

يدرج بعض الأعمدة في ورقة العمل.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, bool updateReference)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود. |
| totalColumns | Int32 | عدد الأعمدة. |
| updateReference | منطقي | يشير إلى ما إذا كانت المراجع في أوراق عمل أخرى سيتم تحديثها. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إدراج 3 أعمدة عند فهرس العمود 2 (بدءًا من الصفر)، مع إزاحة الأعمدة الحالية إلى اليمين
            worksheet.Cells.InsertColumns(2, 3, true);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## InsertColumns(int, int, InsertOptions) {#insertcolumns_1}

يدرج بعض الأعمدة في ورقة العمل.

```csharp
public void InsertColumns(int columnIndex, int totalColumns, InsertOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | Int32 | فهرس العمود. |
| totalColumns | Int32 | عدد الأعمدة. |
| خيارات | InsertOptions | الخيارات لعملية الإدراج. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodInsertColumnsWithInt32Int32InsertOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["C1"].PutValue("Header3");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");
            worksheet.Cells["C2"].PutValue("Data3");

            // إنشاء خيارات الإدراج
            InsertOptions options = new InsertOptions();
            options.CopyFormatType = CopyFormatType.Clear;

            // إدراج عمود عند الفهرس 1 (العمود الثاني)
            worksheet.Cells.InsertColumns(1, 1, options);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


