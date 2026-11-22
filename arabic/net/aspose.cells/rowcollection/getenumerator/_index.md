---
title: "RowCollection.GetEnumerator"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة RowCollection. تحصل على عداد يتنقل عبر الصفوف في هذه المجموعة"
type: docs
url: /ar/net/aspose.cells/rowcollection/getenumerator/
---
## GetEnumerator() {#getenumerator}

يحصل على مُعدِّد يتنقل عبر الصفوف في هذه المجموعة

```csharp
public IEnumerator GetEnumerator()
```

### قيمة الإرجاع

عداد الصفوف الذي سيتنقل عبر جميع الصفوف الموجودة في هذه المجموعة.

### أمثلة

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowCollectionMethodGetEnumeratorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين ارتفاعات الصفوف للعرض
            worksheet.Cells.SetRowHeight(0, 15);
            worksheet.Cells.SetRowHeight(1, 20);
            worksheet.Cells.SetRowHeight(2, 25);

            IEnumerator enumerator = worksheet.Cells.Rows.GetEnumerator();
            while (enumerator.MoveNext())
            {
                Row row = (Row)enumerator.Current;
                Console.WriteLine($"Row index: {row.Index}, Height: {row.Height}");
            }
        }
    }
}
```

### انظر أيضًا

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetEnumerator(bool, bool) {#getenumerator_1}

يحصل على مُعدِّد يتنقل عبر الصفوف في هذه المجموعة

```csharp
public IEnumerator GetEnumerator(bool reversed, bool sync)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| معكوس | منطقي | ما إذا كان سيتم تعداد الصفوف بترتيب معكوس |
| مزامنة | منطقي | ما إذا كان العداد المرتجع يجب أن يتحقق من تعديل مجموعة الصفوف ويحافظ على المزامنة معها. |

### قيمة الإرجاع

عداد الصفوف الذي سيتنقل عبر جميع الصفوف الموجودة في هذه المجموعة.

### ملاحظات

إذا تم تعديل مجموعة الصفوف (بعمليات قد تتسبب في إنشاء Row جديد أو إزالة Row موجود) أثناء التنقل باستخدام العداد، يجب استخدام عداد متزامن بدلاً من العداد العادي بحيث يمكن أن يستمر التنقل من الموضع الذي يلي الأخير الذي تم تنقله بواسطة `MoveNext()`. ومع ذلك، إلى جانب الميزة التي تتمثل في عدم تخطي أي عنصر أو تنقله بشكل متكرر، فإن العيب في العداد المتزامن هو أن الأداء سيتدهور قليلاً مقارنةً بالعداد العادي.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class RowCollectionMethodGetEnumeratorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بعض البيانات النموذجية إلى الصفوف
            for (int i = 0; i < 5; i++)
            {
                Row row = worksheet.Cells.Rows[i];
                row[0].PutValue($"Row {i + 1}");
            }
            
            try
            {
                // الحصول على RowCollection
                RowCollection rows = worksheet.Cells.Rows;
                
                // استدعاء GetEnumerator مع المعلمات (reversed: true, sync: false)
                IEnumerator enumerator = rows.GetEnumerator(true, false);
                
                Console.WriteLine("Iterating rows in reverse order:");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
                
                // استدعاء GetEnumerator مع المعلمات (reversed: false, sync: true)
                enumerator = rows.GetEnumerator(false, true);
                
                Console.WriteLine("\nIterating rows in normal order (synchronized):");
                while (enumerator.MoveNext())
                {
                    Row row = (Row)enumerator.Current;
                    Console.WriteLine(row[0].StringValue);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetEnumerator method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("RowCollectionGetEnumeratorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


