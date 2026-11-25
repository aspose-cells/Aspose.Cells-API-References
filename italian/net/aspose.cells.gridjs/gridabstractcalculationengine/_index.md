---
title: "Classe GridAbstractCalculationEngine"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.GridJs.GridAbstractCalculationEngine class. Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells"
type: docs
url: /it/net/aspose.cells.gridjs/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di **Aspose.Cells**.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridjs/gridabstractcalculationengine/calculate/)(GridCalculationData) | Calcola una funzione con i dati forniti. |

### Osservazioni

L'utente non dovrebbe modificare direttamente alcuna parte della Cartella di lavoro in questa implementazione (eccetto il risultato calcolato della funzione personalizzata, che può essere impostato tramite la proprietà GridCalculationData.CalculatedValue). Altrimenti potrebbero verificarsi risultati inattesi o eccezioni. Se l'utente deve modificare altri dati oltre al risultato calcolato nell'implementazione per alcune funzioni personalizzate, ad esempio modificare la formula di una cella, lo stile, ecc., l'utente dovrebbe raccogliere tali dati in questa implementazione e modificarli al di fuori dell'ambito del calcolo delle formule.

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

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


