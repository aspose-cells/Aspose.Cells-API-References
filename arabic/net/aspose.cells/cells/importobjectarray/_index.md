---
title: "Cells.ImportObjectArray"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تستورد مصفوفة من البيانات إلى ورقة عمل"
type: docs
url: /ar/net/aspose.cells/cells/importobjectarray/
---
## ImportObjectArray(object[], int, int, bool) {#importobjectarray}

يستورد مصفوفة من البيانات إلى ورقة عمل.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| objArray | Object[] | مصفوفة البيانات. |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |
| isVertical | منطقي | يحدد ما إذا كان سيتم استيراد البيانات عموديًا أو أفقيًا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تحضير مصفوفة كائنات ببيانات نموذجية
            object[] dataArray = new object[] { "Product", "Price", "Stock", "Discontinued", 150.5, 75, false };

            try
            {
                // استيراد مصفوفة الكائنات إلى ورقة العمل بدءًا من الخلية B3 (الصف 2، العمود 1)، أفقيًا
                worksheet.Cells.ImportObjectArray(dataArray, 2, 1, false);

                Console.WriteLine("Object array imported successfully to cells B3:F3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // حفظ المصنف لتوضيح النتيجة
            workbook.Save("CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportObjectArray(object[], int, int, bool, int) {#importobjectarray_1}

يستورد مصفوفة من البيانات إلى ورقة عمل.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical, 
    int skip)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| objArray | Object[] | مصفوفة البيانات. |
| firstRow | Int32 | رقم الصف للخلية الأولى التي سيتم الاستيراد فيها. |
| firstColumn | Int32 | رقم العمود للخلية الأولى التي سيتم الاستيراد فيها. |
| isVertical | منطقي | يحدد ما إذا كان سيتم استيراد البيانات عموديًا أو أفقيًا. |
| تخطي | Int32 | عدد الصفوف أو الأعمدة المتخطاة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تحضير البيانات لمعلمات ImportObjectArray: (Object[], Int32, Int32, Boolean, Int32)
            object[] data = new object[]
            {
                "Name",
                "Age",
                "Date",
                "John Doe",
                30,
                new DateTime(2023, 10, 15),
                "Jane Smith",
                28,
                new DateTime(2023, 10, 16)
            };

            try
            {
                // استدعاء ImportObjectArray بالمعلمات: (مصفوفة البيانات، الصف الابتدائي 0، العمود الابتدائي 0، استيراد أفقي، تخطي عمود واحد بين الإدخالات)
                worksheet.Cells.ImportObjectArray(data, 0, 0, false, 1);
                
                Console.WriteLine("Imported object array with parameters (Object[], 0, 0, false, 1) successfully.");
                
                // عرض التأثير: سيتم وضع البيانات في الخلايا A1، C1، E1، A2، C2، E2، إلخ مع تخطي الأعمدة
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportObjectArray: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


