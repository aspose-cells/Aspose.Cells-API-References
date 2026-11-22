---
title: "فئة FindOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.FindOptions. تمثل خيارات البحث"
type: docs
url: /ar/net/aspose.cells/findoptions/
---
## FindOptions class

يمثل خيارات البحث.

```csharp
public class FindOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [FindOptions](findoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CaseSensitive](../../aspose.cells/findoptions/casesensitive/) { get; set; } | يشير إلى ما إذا كانت السلسلة التي تم البحث عنها حساسة لحالة الأحرف. |
| [ConvertNumericData](../../aspose.cells/findoptions/convertnumericdata/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يتم تحويل قيمة السلسلة التي تم البحث عنها إلى بيانات رقمية. |
| [IsCaseSensitive](../../aspose.cells/findoptions/iscasesensitive/) { get; set; } | (**Obsolete.**) يشير إلى ما إذا كانت السلسلة التي تم البحث عنها حساسة لحالة الأحرف. |
| [IsRangeSet](../../aspose.cells/findoptions/israngeset/) { get; } | يشير إلى ما إذا كان النطاق الذي تم البحث فيه محددًا. |
| [LookAtType](../../aspose.cells/findoptions/lookattype/) { get; set; } | انظر إلى النوع. |
| [LookInType](../../aspose.cells/findoptions/lookintype/) { get; set; } | ابحث في النوع. |
| [RegexKey](../../aspose.cells/findoptions/regexkey/) { get; set; } | يشير إلى ما إذا كان المفتاح الذي تم البحث عنه هو تعبير نمطي. إذا كان صحيحًا سيتم اعتبار المفتاح كتعريف نمطي وتحليلّه. وإلا سيتم تحليل المفتاح وفقًا للقواعد في MS Excel. |
| [SearchBackward](../../aspose.cells/findoptions/searchbackward/) { get; set; } | ما إذا كان البحث عكسيًا للخلايا. |
| [SearchNext](../../aspose.cells/findoptions/searchnext/) { get; set; } | (**Obsolete.**) ترتيب البحث. صحيح: البحث عن التالي. خطأ: البحث عن السابق. |
| [SearchOrderByRows](../../aspose.cells/findoptions/searchorderbyrows/) { get; set; } | يشير إلى ما إذا كان ترتيب البحث حسب الصفوف أو الأعمدة. |
| [Style](../../aspose.cells/findoptions/style/) { get; set; } | الصيغة المراد البحث عنها. |
| [ValueTypeSensitive](../../aspose.cells/findoptions/valuetypesensitive/) { get; set; } | يشير إلى ما إذا كان نوع قيمة الخلية التي تم البحث عنها يجب أن يكون مطابقًا للمفتاح الذي تم البحث عنه. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetRange](../../aspose.cells/findoptions/getrange/)() | يحصل ويضبط النطاق الذي تم البحث فيه. |
| [SetRange](../../aspose.cells/findoptions/setrange/)(CellArea) | يضبط النطاق الذي تم البحث فيه. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FindOptionsDemo
    {
        public static void FindOptionsExample()
        {
            // إنشاء كائن دفتر العمل
            Workbook workbook = new Workbook("FindOptionsExample_original.xlsx");

            // الحصول على مجموعة Cells
            Cells cells = workbook.Worksheets[0].Cells;

            // إنشاء كائن FindOptions
            FindOptions findOptions = new FindOptions();

            // إنشاء منطقة Cells
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.StartColumn = 0;
            ca.EndRow = 5;
            ca.EndColumn = 5;

            // تعيين منطقة الخلايا لFindOptions
            findOptions.SetRange(ca);

            // تعيين خصائص البحث
            findOptions.SearchBackward = false;
            findOptions.SearchOrderByRows = true;
            findOptions.LookInType = LookInType.Values;

            // ابحث عن الخلية ذات القيمة 0
            Cell cell = cells.Find(0, null, findOptions);

            if (cell != null)
            {
                Console.WriteLine("Cell found at: " + cell.Name);
            }
            else
            {
                Console.WriteLine("Cell not found.");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


