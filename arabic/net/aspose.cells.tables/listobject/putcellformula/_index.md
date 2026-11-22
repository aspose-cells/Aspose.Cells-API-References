---
title: "ListObject.PutCellFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ListObject. ضع الصيغة في الخلية داخل الجدول"
type: docs
url: /ar/net/aspose.cells.tables/listobject/putcellformula/
---
## PutCellFormula(int, int, string) {#putcellformula}

ضع الصيغة في الخلية داخل الجدول.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | Int32 | إزاحة الصف في الجدول. |
| columnOffset | Int32 | إزاحة العمود في الجدول. |
| صيغة | String | صيغة الخلية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // أضف بيانات عينة لإنشاء جدول
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["C1"].PutValue("Formula");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue(20);

            // إنشاء كائن قائمة (جدول)
            int index = sheet.ListObjects.Add("A1", "C3", true);
            ListObject table = sheet.ListObjects[index];

            // أضف صفًا جديدًا وقم بتعيين القيم/الصيغة
            table.PutCellValue(4, 0, 3); // Row 4, Column 0 (ID)
            table.PutCellValue(4, 1, 30); // Row 4, Column 1 (Value)
            table.PutCellFormula(4, 2, "=B3*2"); // Row 4, Column 2 (Formula)

            // احفظ المصنف
            wb.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellFormula(int, int, string, bool) {#putcellformula_1}

ضع الصيغة في الخلية داخل الجدول.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula, bool isTotalsRowFormula)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | Int32 | إزاحة الصف في الجدول. |
| columnOffset | Int32 | إزاحة العمود في الجدول. |
| صيغة | String | صيغة الخلية. |
| isTotalsRowFormula | منطقي |  |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات عينة لإنشاء كائن قائمة
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // إنشاء كائن قائمة
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // شرح PutCellFormula
            listObject.PutCellFormula(3, 0, "=SUM(A2:A3)", true);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


