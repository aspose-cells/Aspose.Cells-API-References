---
title: "Worksheet.FreezePanes"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تُجمد الألواح عند الخلية المحددة في ورقة العمل"
type: docs
url: /ar/net/aspose.cells/worksheet/freezepanes/
---
## FreezePanes(int, int, int, int) {#freezepanes}

يثبت الألواح عند الخلية المحددة في ورقة العمل.

```csharp
public void FreezePanes(int row, int column, int freezedRows, int freezedColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |
| freezedRows | Int32 | عدد الصفوف الظاهرة في اللوحة العلوية، لا يزيد عن فهرس الصف. |
| freezedColumns | Int32 | عدد الأعمدة الظاهرة في اللوحة اليسرى، لا يزيد عن فهرس العمود. |

### ملاحظات

لا يمكن أن يكون فهرس الصف وفهرس العمود كلاهما صفرًا. كما لا يمكن أن يكون عدد الصفوف وعدد الأعمدة كلاهما صفرًا.

المعاملان الأولان يحددان موضع التجميد، والمعاملان الأخيران يحددان المنطقة المجمدة في اللوحة اليسرى العلوية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // جمد الألواح عند الصف 3، العمود 3، مع 3 صفوف مجمدة و3 أعمدة مجمدة
            worksheet.FreezePanes(3, 3, 3, 3);
            
            // احفظ المصنف
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## FreezePanes(string, int, int) {#freezepanes_1}

يثبت الألواح عند الخلية المحددة في ورقة العمل.

```csharp
public void FreezePanes(string cellName, int freezedRows, int freezedColumns)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم الخلية. |
| freezedRows | Int32 | عدد الصفوف الظاهرة في اللوحة العلوية، لا يزيد عن فهرس الصف. |
| freezedColumns | Int32 | عدد الأعمدة الظاهرة في اللوحة اليسرى، لا يزيد عن فهرس العمود. |

### ملاحظات

لا يمكن أن يكون فهرس الصف وفهرس العمود كلاهما صفرًا. كما لا يمكن أن يكون عدد الصفوف وعدد الأعمدة كلاهما صفرًا.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodFreezePanesWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // جمد الألواح عند "C3" مع 3 صفوف مجمدة و3 أعمدة مجمدة
            worksheet.FreezePanes("C3", 3, 3);

            // احفظ المصنف
            workbook.Save("FreezePanesDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


