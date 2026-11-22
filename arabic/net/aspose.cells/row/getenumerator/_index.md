---
title: "Row.GetEnumerator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Row. يحصل على عداد الخلايا"
type: docs
url: /ar/net/aspose.cells/row/getenumerator/
---
## GetEnumerator() {#getenumerator}

يسترجع عداد الخلايا

```csharp
public IEnumerator GetEnumerator()
```

### قيمة الإرجاع

عداد الخلايا الذي سيتجول عبر جميع الخلايا الموجودة في هذا الصف.

### أمثلة

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // املأ بعض بيانات العينة
            cells["A1"].PutValue("Name");
            cells["B1"].PutValue("Age");
            cells["A2"].PutValue("John");
            cells["B2"].PutValue(30);
            cells["A3"].PutValue("Alice");
            cells["B3"].PutValue(25);

            // احصل على عداد للصف الأول (صف الرأس)
            IEnumerator en = cells.Rows[0].GetEnumerator();
            while (en.MoveNext())
            {
                Cell cell = (Cell)en.Current;
                Console.WriteLine(cell.Name + ": " + cell.Value);
            }
        }
    }
}
```

### انظر أيضًا

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

يسترجع عدادًا يتنقل عبر الخلايا في هذا الصف.

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| معكوس | منطقي | ما إذا كان سيتم تعداد الخلايا بترتيب عكسي |
| مزامنة | منطقي | ما إذا كان يجب على العداد المرتجع فحص تعديل الخلايا في هذا الصف والحفاظ على التزامن معه. |

### قيمة الإرجاع

عداد الخلايا الذي سيتجول عبر جميع الخلايا الموجودة في هذا الصف.

### ملاحظات

إذا تم تعديل الصف (بعمليات قد تتسبب في إنشاء خلية جديدة أو إزالة خلية موجودة) أثناء التجول باستخدام العداد، يجب استخدام عداد متزامن بدلاً من العداد العادي بحيث يمكن للتجول المتابعة من الموضع الذي يلي الأخير الذي تم تجاوزه بواسطة MoveNext() الأخير. ومع ذلك، إلى جانب الميزة التي لا يتم فيها تخطي أي عنصر أو تكرار التجول، فإن العيب في العداد المتزامن هو أن الأداء سيتدهور قليلاً مقارنةً بالعداد العادي.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات إلى الخلايا في الصف الأول
            Row row = worksheet.Cells.Rows[0];
            worksheet.Cells["A1"].PutValue("Cell A1");
            worksheet.Cells["B1"].PutValue("Cell B1");
            worksheet.Cells["C1"].PutValue("Cell C1");

            try
            {
                // استدعِ GetEnumerator مع reversed=false و sync=true
                IEnumerator enumerator = row.GetEnumerator(false, true);
                
                Console.WriteLine("Cells in row 1:");
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }

                // استدعِ GetEnumerator مع reversed=true و sync=false لتوضيح التكرار العكسي
                Console.WriteLine("\nCells in row 1 (reversed order):");
                enumerator = row.GetEnumerator(true, false);
                while (enumerator.MoveNext())
                {
                    Cell cell = (Cell)enumerator.Current;
                    if (cell != null)
                    {
                        Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("RowMethodGetEnumeratorWithBooleanBooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


