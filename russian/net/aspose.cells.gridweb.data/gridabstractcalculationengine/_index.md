---
title: "Класс GridAbstractCalculationEngine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.Data.GridAbstractCalculationEngine. Представляет пользовательский движок расчётов, расширяющий движок расчётов по умолчанию в Aspose.Cells"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Представляет пользовательский движок вычислений, расширяющий движок вычислений по умолчанию в Aspose.Cells.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Методы

| Имя | Описание |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridweb.data/gridabstractcalculationengine/calculate/)(GridCalculationData) | Вычисляет одну функцию с заданными данными. |

### Примеры

```csharp
[C#]
 class MyEngine : GridAbstractCalculationEngine
{
    public override void Calculate(GridCalculationData data)
    {
        string funcName = data.FunctionName.ToUpper();
        if ("MYFUNC".Equals(funcName))
        {
            //выполните вычисление для MYFUNC здесь
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
                //обработайте параметр здесь
                //res = ...;
            }
            data.CalculatedValue = res;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


