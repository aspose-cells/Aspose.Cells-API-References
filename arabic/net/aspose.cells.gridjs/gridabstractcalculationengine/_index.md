---
title: GridAbstractCalculationEngine
second_title: Aspose.Cells لمرجع .NET API
description: يمثل محرك الحساب المخصص للمستخدم لتوسيع محرك الحساب الافتراضي لـ Aspose.Cells.
type: docs
weight: 20
url: /ar/net/aspose.cells.gridjs/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

يمثل محرك الحساب المخصص للمستخدم لتوسيع محرك الحساب الافتراضي لـ Aspose.Cells.

```csharp
public abstract class GridAbstractCalculationEngine
```

## طُرق

| اسم | وصف |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridjs/gridabstractcalculationengine/calculate)(GridCalculationData) | حساب دالة واحدة ببيانات معينة. |

### ملاحظات

يجب ألا يقوم المستخدم بتعديل أي جزء من المصنف مباشرةً في هذا التنفيذ (باستثناء النتيجة المحسوبة للدالة المخصصة ، والتي يمكن تعيينها بواسطة خاصية GridCalculationData.CalculatedValue) . وإلا فقد ينتج عن ذلك نتيجة غير متوقعة أو استثناء . إذا احتاج المستخدم إلى التغيير تؤدي البيانات الأخرى غير المحسوبة إلى تنفيذ بعض الوظائف المخصصة ، على سبيل المثال ، تغيير صيغة الخلية ونمطها ، ... إلخ ، يجب على المستخدم جمع هذه البيانات في هذا التنفيذ وتغييرها خارج نطاق حساب الصيغة.

### أمثلة

```csharp
[C#]
public class MyEngine : GridAbstractCalculationEngine
{
    public override void Calculate(GridCalculationData data)
    {
        string funcName = data.FunctionName.ToUpper();
        if ("MYFUNC".Equals(funcName))
        {
            // قم بحساب MYFUNC هنا
            int count = data.ParamCount;
            object res = null;
            for (int i = 0; i < count; i++)
            {
                object pv = data.GetParamValue(i);
                if (pv is ReferredArea)
                {
                    ReferredArea ra = (ReferredArea)pv;
                    pv = ra.GetValue(0, 0);
                }
                // معالجة المعلمة هنا
                // الدقة = ... ;
            }
            data.CalculatedValue = res;
        }
    }
}
```

### أنظر أيضا

* مساحة الاسم [Aspose.Cells.GridJs](../../aspose.cells.gridjs)
* المجسم [Aspose.Cells.GridJs](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridJs.dll -->
