---
title: "Classe GridAbstractCalculationEngine"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridWeb.Data.GridAbstractCalculationEngine. Représente le moteur de calcul personnalisé des utilisateurs pour étendre le moteur de calcul par défaut d’Aspose.Cells"
type: docs
url: /fr/net/aspose.cells.gridweb.data/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Méthodes

| Nom | Description |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridweb.data/gridabstractcalculationengine/calculate/)(GridCalculationData) | Calcule une fonction avec les données fournies. |

### Exemples

```csharp
[C#]
 class MyEngine : GridAbstractCalculationEngine
{
    public override void Calculate(GridCalculationData data)
    {
        string funcName = data.FunctionName.ToUpper();
        if ("MYFUNC".Equals(funcName))
        {
            //effectuer le calcul pour MYFUNC ici
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
                //traiter le paramètre ici
                //res = ...;
            }
            data.CalculatedValue = res;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


