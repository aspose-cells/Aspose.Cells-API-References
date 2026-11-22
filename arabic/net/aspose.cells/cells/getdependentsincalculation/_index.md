---
title: "Cells.GetDependentsInCalculation"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cells. تحصّل جميع الخلايا التي تعتمد نتيجتها المحسوبة على خلية محددة"
type: docs
url: /ar/net/aspose.cells/cells/getdependentsincalculation/
---
## Cells.GetDependentsInCalculation method

يحصل على جميع الخلايا التي تعتمد نتيجتها المحسوبة على الخلية المحددة.

```csharp
public IEnumerator GetDependentsInCalculation(int row, int column, bool recursive)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف للخلية المحددة |
| عمود | Int32 | فهرس العمود للخلية المحددة. |
| recursive | منطقي | ما إذا كان يُعيد تلك التبعيات التي لا تشير إلى الخلية المحددة مباشرةً بل تشير إلى فروع أخرى لتلك الخلية. |

### قيمة الإرجاع

المُعدد لتعداد جميع التبعيات (كائنات Cell)

### ملاحظات

لاستخدام هذه الطريقة، يرجى التأكد من أن المصنف تم تعيينه بالقيمة true للخاصية [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) وتم حسابه بالكامل باستخدام هذا الإعداد. إذا لم يكن هناك إشارة صيغة إلى هذه الخلية، سيتم إرجاع null. لمزيد من التفاصيل ومثال، يرجى الاطلاع على [`GetDependentsInCalculation`](../../cell/getdependentsincalculation/)

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsMethodGetDependentsInCalculationWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد وحساب الصيغ
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // إعداد تبعيات الصيغ:
            // C1 = 10 (قيمة المصدر)
            // B1 = C1*2
            // A1 = B1+5
            cells["C1"].PutValue(10);
            cells["B1"].Formula = "C1*2";
            cells["A1"].Formula = "B1+5";

            // احسب الصيغ لإنشاء التبعيات
            workbook.CalculateFormula();

            try
            {
                // احصل على التبعيات للخلية C1 (الصف 0، العمود 2) مع فحص تكراري
                IEnumerator dependents = cells.GetDependentsInCalculation(0, 2, true);

                Console.WriteLine("Dependents of cell C1:");
                while (dependents.MoveNext())
                {
                    if (dependents.Current is Cell dependentCell)
                    {
                        Console.WriteLine($"- {dependentCell.Name}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDependentsInCalculation: {ex.Message}");
            }

            // احفظ المصنف
            workbook.Save("GetDependentsInCalculationDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


