---
title: "Row.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Row. تتحقق مما إذا كان هذا الكائن يشير إلى نفس الصف مع آخر"
type: docs
url: /ar/net/aspose.cells/row/equals/
---
## Equals(object) {#equals_1}

يتحقق مما إذا كان هذا الكائن يشير إلى نفس الصف مع آخر.

```csharp
public override bool Equals(object obj)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | Object | كائن آخر |

### قيمة الإرجاع

true إذا كان الكائنان يشيران إلى نفس الصف.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء صفين للمقارنة
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];
            
            // تعيين بعض الخصائص لجعل الصفوف مختلفة
            row1.Height = 20;
            row2.Height = 25;
            
            try
            {
                // استدعاء طريقة Equals مع معامل Object
                bool result1 = row1.Equals((object)row2);
                Console.WriteLine($"Comparing row1 with row2: {result1}");
                
                // قارن row1 بنفسه
                bool result2 = row1.Equals((object)row1);
                Console.WriteLine($"Comparing row1 with itself: {result2}");
                
                // قارن مع null
                bool result3 = row1.Equals((object)null);
                Console.WriteLine($"Comparing row1 with null: {result3}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }
            
            workbook.Save("RowMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Row) {#equals}

يتحقق مما إذا كان هذا الكائن يشير إلى نفس الصف مع كائن صف آخر.

```csharp
public bool Equals(Row row)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Row | كائن صف آخر |

### قيمة الإرجاع

صحيح إذا كان كائني صف يشيران إلى نفس الصف.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowMethodEqualsWithRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء صفين للمقارنة
            Row row1 = worksheet.Cells.Rows[0];
            Row row2 = worksheet.Cells.Rows[1];

            // تعيين بعض الخصائص لجعل الصفوف مختلفة
            row1.Height = 20;
            row2.Height = 25;
            row1.IsHidden = false;
            row2.IsHidden = true;

            try
            {
                // استدعِ طريقة Equals لمقارنة الصفوف
                bool areEqual = row1.Equals(row2);

                // اعرض النتيجة
                Console.WriteLine($"Are rows equal? {areEqual}");

                // أنشئ صفًا آخر بنفس الخصائص مثل row1
                Row row3 = worksheet.Cells.Rows[2];
                row3.Height = row1.Height;
                row3.IsHidden = row1.IsHidden;

                // قارن row1 مع row3 (يجب أن تكون متساوية)
                bool areEqual2 = row1.Equals(row3);
                Console.WriteLine($"Are rows equal after matching properties? {areEqual2}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("RowEqualsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


