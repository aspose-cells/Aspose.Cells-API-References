---
title: "Cell.Equals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع كائن آخر"
type: docs
url: /ar/net/aspose.cells/cell/equals/
---
## Equals(object) {#equals_1}

يتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع آخر.

```csharp
public override bool Equals(object obj)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | Object | كائن آخر |

### قيمة الإرجاع

صحيح إذا كان الكائنان يشيران إلى نفس الخلية.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى خلايا من مواقع مختلفة
            Cell cellA1 = worksheet.Cells["A1"];
            Cell anotherCellA1 = worksheet.Cells[0, 0]; // Same physical cell as A1
            Cell cellB1 = worksheet.Cells["B1"];

            // تعيين قيم متطابقة في خلايا مختلفة
            cellA1.PutValue("Aspose.Cells");
            cellB1.PutValue("Aspose.Cells");

            try
            {
                // مقارنة مراجع الخلايا الفيزيائية نفسها
                bool sameCellComparison = cellA1.Equals(anotherCellA1);
                Console.WriteLine($"Same cell comparison: {sameCellComparison}"); // True

                // قارن الخلايا المختلفة ذات المحتوى المتطابق
                bool differentCellComparison = cellA1.Equals(cellB1);
                Console.WriteLine($"Different cell comparison: {differentCellComparison}"); // False

                // قارن الخلية مع كائن غير خلية
                bool invalidTypeComparison = cellA1.Equals("Aspose.Cells");
                Console.WriteLine($"Invalid type comparison: {invalidTypeComparison}"); // False
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("CellMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Cell) {#equals}

يتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع كائن خلية آخر.

```csharp
public bool Equals(Cell cell)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خلية | خلية | كائن خلية آخر |

### قيمة الإرجاع

صحيح إذا كان كائنان للخلية يشيران إلى نفس الخلية.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithCellDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء خلايا في مواقع مختلفة (A1 و B1)
            Cell cellA1 = worksheet.Cells[0, 0];
            Cell cellB1 = worksheet.Cells[0, 1];

            // تعيين قيم متطابقة في كلتا الخليتين
            cellA1.Value = "Aspose.Cells Comparison";
            cellB1.Value = "Aspose.Cells Comparison";

            try
            {
                // قارن cellA1 مع cellB1 (مواقع مختلفة)
                bool equalsResult = cellA1.Equals(cellB1);
                Console.WriteLine($"Cell A1 equals Cell B1: {equalsResult}");

                // قارن cellA1 مع نفسه (نفس المثيل)
                equalsResult = cellA1.Equals(cellA1);
                Console.WriteLine($"Cell A1 equals itself: {equalsResult}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("CellMethodEqualsWithCellDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


