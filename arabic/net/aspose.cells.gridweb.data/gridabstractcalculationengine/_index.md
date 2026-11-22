---
title: "الفئة GridAbstractCalculationEngine"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.GridWeb.Data.GridAbstractCalculationEngine. تمثل محرك حساب مخصص للمستخدمين لتوسيع محرك الحساب الافتراضي لـ Aspose.Cells"
type: docs
url: /ar/net/aspose.cells.gridweb.data/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

يمثل محرك الحساب المخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells.

```csharp
public abstract class GridAbstractCalculationEngine
```

## الطرق

| الاسم | الوصف |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridweb.data/gridabstractcalculationengine/calculate/)(GridCalculationData) | يحسب دالة واحدة باستخدام البيانات المعطاة. |

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

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


