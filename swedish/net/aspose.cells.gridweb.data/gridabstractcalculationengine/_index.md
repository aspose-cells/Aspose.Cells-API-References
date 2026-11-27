---
title: "Klass GridAbstractCalculationEngine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridWeb.Data.GridAbstractCalculationEngine-klass. Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells"
type: docs
url: /sv/net/aspose.cells.gridweb.data/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridweb.data/gridabstractcalculationengine/calculate/)(GridCalculationData) | Beräknar en funktion med angivna data. |

### Exempel

```csharp
[C#]
 class MyEngine : GridAbstractCalculationEngine
{
    public override void Calculate(GridCalculationData data)
    {
        string funcName = data.FunctionName.ToUpper();
        if ("MYFUNC".Equals(funcName))
        {
            //utför beräkning för MYFUNC här
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
                //processa parametern här
                //res = ...;
            }
            data.CalculatedValue = res;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


