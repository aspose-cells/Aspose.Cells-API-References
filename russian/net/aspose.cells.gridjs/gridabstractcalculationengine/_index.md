---
title: "Класс GridAbstractCalculationEngine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridJs.GridAbstractCalculationEngine class. Представляет пользовательский движок расчётов, расширяющий движок расчётов по умолчанию Aspose.Cells"
type: docs
url: /ru/net/aspose.cells.gridjs/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Представляет пользовательский движок вычислений, расширяющий движок вычислений по умолчанию в Aspose.Cells.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Методы

| Имя | Описание |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridjs/gridabstractcalculationengine/calculate/)(GridCalculationData) | Вычисляет одну функцию с заданными данными. |

### Примечания

Пользователь не должен изменять любую часть Workbook напрямую в этой реализации (за исключением вычисленного результата пользовательской функции, который можно задать через свойство GridCalculationData.CalculatedValue). В противном случае могут возникнуть неожиданные результаты или Exception. Если пользователю необходимо изменить другие данные, помимо вычисленного результата, в реализации для некоторых пользовательских функций, например изменить формулу ячейки, стиль и т.д., пользователь должен собрать эти данные в этой реализации и изменить их вне области расчёта формул.

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

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


