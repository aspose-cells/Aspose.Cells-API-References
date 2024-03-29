---
title: AbstractCalculationEngine
second_title: Riferimento alle API di Aspose.Cells per .NET
description: Rappresenta il motore di calcolo personalizzato dellutente per estendere il motore di calcolo predefinito di Aspose.Cells.
type: docs
weight: 20
url: /it/net/aspose.cells/abstractcalculationengine/
---
## AbstractCalculationEngine class

Rappresenta il motore di calcolo personalizzato dell'utente per estendere il motore di calcolo predefinito di Aspose.Cells.

```csharp
public abstract class AbstractCalculationEngine
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [IsParamLiteralRequired](../../aspose.cells/abstractcalculationengine/isparamliteralrequired) { get; } | Indica se questo motore necessita del testo letterale del parametro durante l'esecuzione del calcolo. Il valore predefinito è false. |
| virtual [ProcessBuiltInFunctions](../../aspose.cells/abstractcalculationengine/processbuiltinfunctions) { get; } | Se le funzioni integrate che sono state supportate dal motore integrato devono essere controllate ed elaborate da questa implementazione. L'impostazione predefinita è false. Se l'utente deve modificare la logica di calcolo di alcune funzioni integrate, questa proprietà dovrebbe essere impostato come vero. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| abstract [Calculate](../../aspose.cells/abstractcalculationengine/calculate)(CalculationData) | Calcola una funzione con dati dati. |

### Osservazioni

L'utente non deve modificare alcuna parte della cartella di lavoro direttamente in questa implementazione (tranne il risultato calcolato della funzione personalizzata, che può essere impostato dalla proprietà CalculationData.CalculatedValue). In caso contrario potrebbero verificarsi risultati imprevisti o eccezioni. Se l'utente deve modificare dati diversi da quelli calcolati risultano nell'implementazione per alcune funzioni personalizzate, ad esempio , modifica la formula della cella, lo stile, ecc., l'utente dovrebbe raccogliere quei dati in questa implementazione e cambiarli fuori dall'ambito del calcolo della formula.

### Esempi

```csharp
[C#]
public class MyEngine : AbstractCalculationEngine
{
    public override void Calculate(CalculationData data)
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

* spazio dei nomi [Aspose.Cells](../../aspose.cells)
* assemblea [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
