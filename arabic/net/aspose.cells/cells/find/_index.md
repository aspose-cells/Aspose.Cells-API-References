---
title: "Cells.Find"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تبحث عن الخلية التي تحتوي على الكائن المدخل"
type: docs
url: /ar/net/aspose.cells/cells/find/
---
## Find(object, Cell) {#find}

يبحث عن الخلية التي تحتوي على الكائن المدخل.

```csharp
public Cell Find(object what, Cell previousCell)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ماذا | Object | الكائن المراد البحث عنه. يجب أن يكون النوع int,double,DateTime,string,bool. |
| previousCell | خلية | الخلية السابقة التي تحتوي على نفس الكائن. يمكن تعيين هذه المعلمة إلى null إذا كان البحث من البداية. |

### قيمة الإرجاع

كائن الخلية.

### ملاحظات

يعيد null (Nothing) إذا لم يتم العثور على أي خلية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1.2);

            // ابحث عن الخلية التي تحتوي على "Orange"
            Cell searchCell = null;
            Cell foundCell = worksheet.Cells.Find("Orange", searchCell);

            if (foundCell != null)
            {
                Console.WriteLine("Found 'Orange' at: " + foundCell.Name);
                
                // إنشاء وتطبيق نمط على الخلية التي تم العثور عليها
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Red;
                style.Font.IsBold = true;
                foundCell.SetStyle(style);
            }

            // احفظ المصنف
            workbook.Save("FindMethodDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Find(object, Cell, FindOptions) {#find_1}

يبحث عن الخلية التي تحتوي على الكائن المدخل.

```csharp
public Cell Find(object what, Cell previousCell, FindOptions findOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ماذا | Object | الكائن المراد البحث عنه. يجب أن يكون النوع int,double,DateTime,string,bool. |
| previousCell | خلية | الخلية السابقة التي تحتوي على نفس الكائن. يمكن تعيين هذه المعلمة إلى null إذا كان البحث من البداية. |
| findOptions | FindOptions | خيارات البحث |

### قيمة الإرجاع

كائن الخلية.

### ملاحظات

يعيد null (Nothing) إذا لم يتم العثور على أي خلية.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellFindOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين بيانات عينة
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["A2"].PutValue("def");
            worksheet.Cells["A3"].PutValue("abc ");
            
            // إنشاء خيارات البحث
            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // ابحث عن الخلية ذات القيمة "abc "
            Cell foundCell = worksheet.Cells.Find("abc ", null, options);
            
            Console.WriteLine("Found cell: " + (foundCell != null ? foundCell.Name : "null"));
        }
    }
}
```

### انظر أيضًا

* class [Cell](../../cell/)
* class [FindOptions](../../findoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


