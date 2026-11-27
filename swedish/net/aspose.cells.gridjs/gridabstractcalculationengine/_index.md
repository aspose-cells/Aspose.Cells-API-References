---
title: "Klass GridAbstractCalculationEngine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.GridJs.GridAbstractCalculationEngine-klass. Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells"
type: docs
url: /sv/net/aspose.cells.gridjs/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Representerar användarens anpassade beräkningsmotor för att utöka standardberäkningsmotorn i Aspose.Cells.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridjs/gridabstractcalculationengine/calculate/)(GridCalculationData) | Beräknar en funktion med angivna data. |

### Anmärkningar

Användaren bör inte ändra någon del av arbetsboken direkt i denna implementation (förutom det beräknade resultatet av den anpassade funktionen, som kan sättas via egenskapen GridCalculationData.CalculatedValue). Annars kan oväntade resultat eller undantag uppstå. Om användaren behöver ändra annan data än det beräknade resultatet i implementationen för vissa anpassade funktioner, till exempel ändra cellens formel, stil, ...etc., bör användaren samla in dessa data i implementationen och ändra dem utanför formelberäkningens område.

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

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


