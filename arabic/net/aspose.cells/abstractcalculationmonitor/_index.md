---
title: AbstractCalculationMonitor
second_title: Aspose.Cells لمرجع .NET API
description: مراقبة للمستخدم لتتبع تقدم حساب الصيغة.
type: docs
weight: 30
url: /ar/net/aspose.cells/abstractcalculationmonitor/
---
## AbstractCalculationMonitor class

مراقبة للمستخدم لتتبع تقدم حساب الصيغة.

```csharp
public abstract class AbstractCalculationMonitor
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [CalculatedValue](../../aspose.cells/abstractcalculationmonitor/calculatedvalue) { get; } | الحصول على القيمة المحسوبة حديثًا للخلية . يجب استخدامه فقط في[`AfterCalculate`](./aftercalculate) . |
| [OriginalValue](../../aspose.cells/abstractcalculationmonitor/originalvalue) { get; } | الحصول على القيمة القديمة للخلية المحسوبة. يجب استخدامه فقط في[`BeforeCalculate`](./beforecalculate) و[`AfterCalculate`](./aftercalculate) . |
| [ValueChanged](../../aspose.cells/abstractcalculationmonitor/valuechanged) { get; } | ما إذا كانت قيمة الخلية قد تغيرت بعد الحساب. يجب استخدامها فقط في[`AfterCalculate`](./aftercalculate) . |

## طُرق

| اسم | وصف |
| --- | --- |
| virtual [AfterCalculate](../../aspose.cells/abstractcalculationmonitor/aftercalculate)(int, int, int) | قم بتنفيذ هذه الطريقة لممارسة الأعمال التجارية بعد حساب خلية واحدة. |
| virtual [BeforeCalculate](../../aspose.cells/abstractcalculationmonitor/beforecalculate)(int, int, int) | قم بتنفيذ هذه الطريقة للقيام بالأعمال قبل حساب خلية واحدة. |
| virtual [OnCircular](../../aspose.cells/abstractcalculationmonitor/oncircular)(IEnumerator) | قم بتنفيذ هذه الطريقة للقيام بالأعمال عند حساب الصيغ ذات المراجع الدائرية. |

### أمثلة

```csharp
[C#]
// شاشة مخصصة للتحقق من إمكانية StackOverflowException
public class MyCalculationMonitor : AbstractCalculationMonitor
{
    public override void BeforeCalculate(int sheetIndex, int rowIndex, int colIndex)
    {
        if(new StackTrace(false).FrameCount > 1000)
        {
            throw new Exception("Stop the formula calculation because risk of StackOverflowException");
        }
    }
}
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells](../../aspose.cells)
* المجسم [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->