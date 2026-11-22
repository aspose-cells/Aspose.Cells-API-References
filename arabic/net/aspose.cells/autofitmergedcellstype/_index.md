---
title: "تعداد AutoFitMergedCellsType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.AutoFitMergedCellsType. يمثل نوع تعديل حجم الخلايا المدمجة تلقائيًا"
type: docs
url: /ar/net/aspose.cells/autofitmergedcellstype/
---
## AutoFitMergedCellsType enumeration

يمثل نوع الضبط التلقائي للخلايا المدمجة.

```csharp
public enum AutoFitMergedCellsType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | تجاهل الخلايا المدمجة. |
| FirstLine | `1` | يقوم فقط بتوسيع ارتفاع الصف الأول. |
| LastLine | `2` | يقوم فقط بتوسيع ارتفاع الصف الأخير. |
| EachLine | `3` | يقوم بتوسيع ارتفاع كل صف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;

    public class AutoFitMergedCellsTypeDemo
    {
        public static void AutoFitMergedCellsTypeExample()
        {
            //إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            //الحصول على مرجع ورقة العمل المضافة حديثًا
            Worksheet sheet1 = workbook.Worksheets[0];

            // إنشاء نطاق A1:B2
            Range range = sheet1.Cells.CreateRange(0, 0, 2, 2);

            // دمج الخلايا
            range.Merge();

            // إدراج قيمة في الخلية المدمجة A1
            sheet1.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // إنشاء كائن نمط
            Style style = sheet1.Cells[0, 0].GetStyle();

            // تفعيل التفاف النص
            style.IsTextWrapped = true;

            // تطبيق النمط على الخلية
            sheet1.Cells[0, 0].SetStyle(style);

            // إنشاء كائن لـ AutoFitterOptions
            AutoFitterOptions options = new AutoFitterOptions();

            // يقوم فقط بتوسيع ارتفاع الصف الأول.
            options.AutoFitMergedCellsType = AutoFitMergedCellsType.FirstLine;

            // تعديل حجم الصفوف تلقائيًا في الورقة (بما في ذلك الخلايا المدمجة)
            sheet1.AutoFitRows(options);


            int index = workbook.Worksheets.Add();
            Worksheet sheet2 = workbook.Worksheets[index];
            sheet2.Name = "Sheet2";
            // إنشاء نطاق A1:B2
            Range range2 = sheet2.Cells.CreateRange(0, 0, 2, 2);

            // دمج الخلايا
            range2.Merge();

            // إدراج قيمة في الخلية المدمجة A1
            sheet2.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // إنشاء كائن نمط
            Style style2 = sheet2.Cells[0, 0].GetStyle();

            // تفعيل التفاف النص
            style2.IsTextWrapped = true;

            // تطبيق النمط على الخلية
            sheet2.Cells[0, 0].SetStyle(style);

            // إنشاء كائن لـ AutoFitterOptions
            AutoFitterOptions options2 = new AutoFitterOptions();

            // يقوم فقط بتوسيع ارتفاع الصف الأخير.
            options2.AutoFitMergedCellsType = AutoFitMergedCellsType.LastLine;

            // تعديل حجم الصفوف تلقائيًا في الورقة (بما في ذلك الخلايا المدمجة)
            sheet2.AutoFitRows(options2);


            index = workbook.Worksheets.Add();
            Worksheet sheet3 = workbook.Worksheets[index];
            sheet3.Name = "Sheet3";
            // إنشاء نطاق A1:B2
            Range range3 = sheet3.Cells.CreateRange(0, 0, 2, 2);

            // دمج الخلايا
            range3.Merge();

            // إدراج قيمة في الخلية المدمجة A1
            sheet3.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // إنشاء كائن نمط
            Style style3 = sheet3.Cells[0, 0].GetStyle();

            // تفعيل التفاف النص
            style3.IsTextWrapped = true;

            // تطبيق النمط على الخلية
            sheet3.Cells[0, 0].SetStyle(style);

            // إنشاء كائن لـ AutoFitterOptions
            AutoFitterOptions options3 = new AutoFitterOptions();

            // يقوم فقط بتوسيع ارتفاع كل صف.
            options3.AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine;

            // تعديل حجم الصفوف تلقائيًا في الورقة (بما في ذلك الخلايا المدمجة)
            sheet3.AutoFitRows(options3);


            index = workbook.Worksheets.Add();
            Worksheet sheet4 = workbook.Worksheets[index];
            sheet4.Name = "Sheet4";
            // إنشاء نطاق A1:B2
            Range range4 = sheet4.Cells.CreateRange(0, 0, 2, 2);

            // دمج الخلايا
            range4.Merge();

            // إدراج قيمة في الخلية المدمجة A1
            sheet4.Cells[0, 0].Value = "This is test text for autofit merged cells type demo This is test text for autofit merged cells type demo";

            // إنشاء كائن نمط
            Style style4 = sheet4.Cells[0, 0].GetStyle();

            // تفعيل التفاف النص
            style4.IsTextWrapped = true;

            // تطبيق النمط على الخلية
            sheet4.Cells[0, 0].SetStyle(style);

            // إنشاء كائن لـ AutoFitterOptions
            AutoFitterOptions options4 = new AutoFitterOptions();

            // تجاهل الخلايا المدمجة.
            options4.AutoFitMergedCellsType = AutoFitMergedCellsType.None;

            // تعديل حجم الصفوف تلقائيًا في الورقة (دون تضمين الخلايا المدمجة)
            sheet4.AutoFitRows(options4);

            // احفظ المصنف
            workbook.Save("AutoFitMergedCellsTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


