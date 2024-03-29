---
title: GridAbstractCalculationEngine
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta il motore di calcolo personalizzato dellutente per estendere il motore di calcolo predefinito di Aspose.Cells.
type: docs
weight: 130
url: /it/net/aspose.cells.gridweb.data/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridweb.data/gridabstractcalculationengine/calculate)(GridCalculationData) | Calcola una funzione con dati dati. |

### Esempi

```csharp
[C#]
public class MyEngine : GridAbstractCalculationEngine
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
                if (pv is ReferredArea)
                {
                    ReferredArea ra = (ReferredArea)pv;
                    pv = ra.GetValue(0, 0);
                }
                //elabora il parametro qui
                //risp = ...;
            }
            data.CalculatedValue = res;
        }
    }
}
```

### Guarda anche

* spazio dei nomi [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* assemblea [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
