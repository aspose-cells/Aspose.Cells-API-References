---
title: "ListObjectCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ListObjectCollection. تضيف ListObject إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.tables/listobjectcollection/add/
---
## Add(int, int, int, int, bool) {#add}

يضيف ListObject إلى ورقة العمل.

```csharp
public int Add(int startRow, int startColumn, int endRow, int endColumn, bool hasHeaders)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | Int32 | صف البداية لنطاق القائمة. |
| startColumn | Int32 | صف البداية لنطاق القائمة. |
| endRow | Int32 | صف البداية لنطاق القائمة. |
| endColumn | Int32 | صف البداية لنطاق القائمة. |
| hasHeaders | منطقي | ما إذا كان النطاق يحتوي على رؤوس. |

### قيمة الإرجاع

فهرس ListObject الجديد

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء البيانات في نطاق
            var range = worksheet.Cells.CreateRange("B3:D4");
            range.Value = new object[,]
            {
                {"Col1", "Col2", "Col3"},
                {100, 200, 300}
            };

            // إضافة ListObject باستخدام طريقة Add مع معلمات Int32
            int firstRow = range.FirstRow;
            int firstColumn = range.FirstColumn;
            int endRow = firstRow + range.RowCount - 1;
            int endColumn = firstColumn + range.ColumnCount - 1;
            worksheet.ListObjects.Add(firstRow, firstColumn, endRow, endColumn, true);

            // تمكين الإجماليات وتعيين الصيغة لعمود واحد
            worksheet.ListObjects[0].ShowTotals = true;
            worksheet.Cells["D5"].Formula = "=SUBTOTAL(109,[Col3])";

            // احفظ المصنف
            workbook.Save("ListObjectAddDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, bool) {#add_1}

يضيف ListObject إلى ورقة العمل.

```csharp
public int Add(string startCell, string endCell, bool hasHeaders)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| startCell | String | خلية البداية لنطاق القائمة. |
| endCell | String | خلية النهاية لنطاق القائمة. |
| hasHeaders | منطقي | ما إذا كان النطاق يحتوي على رؤوس. |

### قيمة الإرجاع

فهرس ListObject الجديد

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectCollectionMethodAddWithStringStringBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء بيانات عينة
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B3"].PutValue(4);

            // إضافة ListObject باستخدام مراجع نطاق السلسلة
            ListObjectCollection listObjects = worksheet.ListObjects;
            listObjects.Add("A1", "B3", true);
            
            workbook.Save("ListObjectExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListObjectCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


