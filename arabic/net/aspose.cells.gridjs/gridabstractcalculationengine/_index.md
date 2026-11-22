---
title: "الفئة GridAbstractCalculationEngine"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.GridJs.GridAbstractCalculationEngine. تمثل محرك حساب مخصص للمستخدمين لتوسيع محرك الحساب الافتراضي في Aspose.Cells"
type: docs
url: /ar/net/aspose.cells.gridjs/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

يمثل محرك الحساب المخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells.

```csharp
public abstract class GridAbstractCalculationEngine
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridjs/gridabstractcalculationengine/calculate/)(GridCalculationData) | يحسب دالة واحدة باستخدام البيانات المعطاة. |

### ملاحظات

يجب على المستخدم عدم تعديل أي جزء من دفتر العمل مباشرةً في هذا التنفيذ (باستثناء النتيجة المحسوبة للدالة المخصصة، والتي يمكن تعيينها عبر الخاصية GridCalculationData.CalculatedValue). وإلا قد يحدث نتيجة غير متوقعة أو استثناء. إذا كان المستخدم بحاجة إلى تغيير بيانات أخرى غير النتيجة المحسوبة في التنفيذ لبعض الدوال المخصصة، على سبيل المثال تغيير صيغة الخلية أو نمطها، ... إلخ، يجب على المستخدم جمع تلك البيانات في هذا التنفيذ وتغييرها خارج نطاق حساب الصيغ.

### أمثلة

```csharp
[C#]
 class MyEngine : GridAbstractCalculationEngine
{
    public override void Calculate(GridCalculationData data)
    {
        string funcName = data.FunctionName.ToUpper();
        if ("MYFUNC".Equals(funcName))
        {   
            //قم بالحساب لـ MYFUNC هنا
            int count = data.ParamCount;
            object res = null;
            for (int i = 0; i < count; i++)
            {
                object pv = data.GetParamValue(i);
                if (pv is GridReferredArea)
                {
                    GridReferredArea ra = (GridReferredArea)pv;
                    pv = ra.GetValue(0, 0);
                }
                //معالجة المعامل هنا
                //res = ...;
            }
            data.CalculatedValue = res;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


