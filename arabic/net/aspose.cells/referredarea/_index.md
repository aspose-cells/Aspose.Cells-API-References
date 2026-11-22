---
title: "Class ReferredArea"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.ReferredArea class. يمثل منطقة مُشار إليها بالصيغة"
type: docs
url: /ar/net/aspose.cells/referredarea/
---
## ReferredArea class

يمثل منطقة مُشار إليها بواسطة الصيغة.

```csharp
public class ReferredArea
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [EndColumn](../../aspose.cells/referredarea/endcolumn/) { get; } | عمود النهاية للمنطقة. |
| [EndRow](../../aspose.cells/referredarea/endrow/) { get; } | صف النهاية للمنطقة. |
| [ExternalFileName](../../aspose.cells/referredarea/externalfilename/) { get; } | احصل على اسم الملف الخارجي إذا كان هذا إشارة خارجية. |
| [IsArea](../../aspose.cells/referredarea/isarea/) { get; } | يشير إلى ما إذا كان هذا منطقة. |
| [IsEntireColumn](../../aspose.cells/referredarea/isentirecolumn/) { get; } | يشير إلى ما إذا كانت هذه المنطقة تحتوي على جميع الصفوف (عمود كامل). |
| [IsEntireRow](../../aspose.cells/referredarea/isentirerow/) { get; } | يشير إلى ما إذا كانت هذه المنطقة تحتوي على جميع الأعمدة (صف كامل). |
| [IsExternalLink](../../aspose.cells/referredarea/isexternallink/) { get; } | يشير إلى ما إذا كان هذا رابطًا خارجيًا. |
| [SheetName](../../aspose.cells/referredarea/sheetname/) { get; } | يشير إلى الورقة التي توجد فيها هذه الإشارة. |
| [SheetNames](../../aspose.cells/referredarea/sheetnames/) { get; } | أسماء جميع أوراق العمل التي يشير إليها هذا الكائن. |
| [StartColumn](../../aspose.cells/referredarea/startcolumn/) { get; } | عمود البداية للمنطقة. |
| [StartRow](../../aspose.cells/referredarea/startrow/) { get; } | صف البداية للمنطقة. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue)(int, int) | يحصل على قيمة الخلية مع الإزاحة المحددة من أعلى اليسار لهذه المنطقة. |
| [GetValue](../../aspose.cells/referredarea/getvalue/#getvalue_1)(int, int, bool) | يحصل على قيمة الخلية مع الإزاحة المحددة من أعلى اليسار لهذه المنطقة. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues)() | يحصل على قيم الخلايا في هذه المنطقة. |
| [GetValues](../../aspose.cells/referredarea/getvalues/#getvalues_1)(bool) | يحصل على قيم الخلايا في هذه المنطقة. |
| override [ToString](../../aspose.cells/referredarea/tostring/)() | يرجع عنوان الإشارة لهذه المنطقة. عادةً ما يكون عنوان الإشارة الذي يمكن استخدامه في الصيغة، مثل "Sheet1!A1:C3". |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassReferredAreaDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد للعرض
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // قم بإعداد بعض البيانات وصيغة تشير إلى نطاق
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["B1"].PutValue(30);
                worksheet.Cells["B2"].PutValue(40);

                // أنشئ صيغة تشير إلى النطاق A1:B2
                Cell formulaCell = worksheet.Cells["C1"];
                formulaCell.Formula = "=SUM(A1:B2)";

                // احصل على المناطق المشار إليها من الصيغة
                ReferredAreaCollection referredAreas = formulaCell.GetPrecedents();
                if (referredAreas.Count > 0)
                {
                    // احصل على أول منطقة مشار إليها
                    ReferredArea referredArea = referredAreas[0];

                    // اعرض الخصائص الأساسية للمنطقة المشار إليها
                    Console.WriteLine($"Referred Area Details:");
                    Console.WriteLine($"- Is External Link: {referredArea.IsExternalLink}");
                    Console.WriteLine($"- Sheet Name: {referredArea.SheetName}");
                    Console.WriteLine($"- Start Row: {referredArea.StartRow}");
                    Console.WriteLine($"- Start Column: {referredArea.StartColumn}");
                    Console.WriteLine($"- End Row: {referredArea.EndRow}");
                    Console.WriteLine($"- End Column: {referredArea.EndColumn}");
                    Console.WriteLine($"- Is Area: {referredArea.IsArea}");
                    Console.WriteLine($"- Is Entire Row: {referredArea.IsEntireRow}");
                    Console.WriteLine($"- Is Entire Column: {referredArea.IsEntireColumn}");

                    // احصل على القيم من المنطقة المشار إليها
                    object values = referredArea.GetValues();
                    if (values is Array)
                    {
                        object[][] valueArray = (object[][])values;
                        Console.WriteLine("\nValues in the referred area:");
                        foreach (object[] row in valueArray)
                        {
                            foreach (object val in row)
                            {
                                Console.Write($"{val}\t");
                            }
                            Console.WriteLine();
                        }
                    }

                    // احصل على قيمة محددة من المنطقة المشار إليها
                    object specificValue = referredArea.GetValue(0, 1);
                    Console.WriteLine($"\nValue at row 0, column 1: {specificValue}");

                    // اعرض عنوان الإشارة
                    Console.WriteLine($"Reference address: {referredArea.ToString()}");
                }

                // احفظ المصنف
                workbook.Save("ReferredAreaDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ReferredArea: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


