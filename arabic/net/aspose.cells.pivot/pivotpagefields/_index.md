---
title: "الفئة PivotPageFields"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Pivot.PivotPageFields. تمثل عناصر صفحة pivot إذا كان مصدر بيانات جدول pivot هو نطاقات التجميع. يمكن أن تحتوي على ما يصل إلى 4 عناصر فقط"
type: docs
url: /ar/net/aspose.cells.pivot/pivotpagefields/
---
## PivotPageFields class

يمثل عناصر صفحة المحور إذا كان مصدر بيانات جدول محوري هو نطاقات تجميع. يمكن أن يحتوي على ما يصل إلى 4 عناصر فقط.

```csharp
public class PivotPageFields
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [PivotPageFields](pivotpagefields/)() | تمثل عناصر حقل صفحة pivot. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [PageFieldCount](../../aspose.cells.pivot/pivotpagefields/pagefieldcount/) { get; } | يحصل على عدد حقول الصفحة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [AddIdentify](../../aspose.cells.pivot/pivotpagefields/addidentify/)(int, int[]) | يضبط أي تسمية عنصر في كل حقل صفحة لاستخدامها لتحديد نطاق البيانات. يجب أن يكون طول pageItemIndex مساويًا لـ PageFieldCount، لذا يرجى إضافة حقل الصفحة أولاً. |
| [AddPageField](../../aspose.cells.pivot/pivotpagefields/addpagefield/)(string[]) | يضيف حقل صفحة. |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotPageFieldsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            Worksheet sheet1 = workbook.Worksheets[0];
            sheet1.Name = "Sheet1";
            FillData(sheet1);

            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            FillData(sheet2);

            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            PivotTableCollection pivotTables = pivotSheet.PivotTables;

            string[] src = { "=Sheet1!A1:C8", "=Sheet2!A1:C8" };
            PivotPageFields pageFields = new PivotPageFields();

            pageFields.AddPageField(new string[] { "item1", "item2" });
            pageFields.AddPageField(new string[] { "item3", "item4" });

            pageFields.AddIdentify(0, new int[] { 0, 1 });
            pageFields.AddIdentify(1, new int[] { 1, -1 });

            pivotTables.Add(src, false, pageFields, "E3", "PivotTable1");

            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }

        private static void FillData(Worksheet sheet)
        {
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["B1"].PutValue("Value");
            cells["C1"].PutValue("Date");

            for (int i = 1; i < 8; i++)
            {
                cells[$"A{i+1}"].PutValue($"Item{i}");
                cells[$"B{i+1}"].PutValue(i * 100);
                cells[$"C{i+1}"].PutValue(System.DateTime.Now.AddDays(i).ToString("yyyy-MM-dd"));
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


