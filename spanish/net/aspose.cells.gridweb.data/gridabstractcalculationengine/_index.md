---
title: "Clase GridAbstractCalculationEngine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.GridWeb.Data.GridAbstractCalculationEngine. Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells"
type: docs
url: /es/net/aspose.cells.gridweb.data/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Representa el motor de cálculo personalizado del usuario para ampliar el motor de cálculo predeterminado de Aspose.Cells.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridweb.data/gridabstractcalculationengine/calculate/)(GridCalculationData) | Calcula una función con los datos proporcionados. |

### Ejemplos

```csharp
[C#]
 class MyEngine : GridAbstractCalculationEngine
{
    public override void Calculate(GridCalculationData data)
    {
        string funcName = data.FunctionName.ToUpper();
        if ("MYFUNC".Equals(funcName))
        {
            //realizar cálculo para MYFUNC aquí
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
                //procesar el parámetro aquí
                //res = ...;
            }
            data.CalculatedValue = res;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


