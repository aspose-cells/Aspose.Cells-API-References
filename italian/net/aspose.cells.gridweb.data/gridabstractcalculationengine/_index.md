---
title: "Classe GridAbstractCalculationEngine"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.GridWeb.Data.GridAbstractCalculationEngine. Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells"
type: docs
url: /it/net/aspose.cells.gridweb.data/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di **Aspose.Cells**.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridweb.data/gridabstractcalculationengine/calculate/)(GridCalculationData) | Calcola una funzione con i dati forniti. |

### Esempi

```csharp
[C#]
 class MyEngine : GridAbstractCalculationEngine
{
    public override void Calculate(GridCalculationData data)
    {
        string funcName = data.FunctionName.ToUpper();
        if ("MYFUNC".Equals(funcName))
        {
            //esegui il calcolo per MYFUNC qui
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
                //elabora il parametro qui
                //res = ...;
            }
            data.CalculatedValue = res;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


