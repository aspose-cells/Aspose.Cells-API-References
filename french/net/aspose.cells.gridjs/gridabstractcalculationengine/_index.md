---
title: "Classe GridAbstractCalculationEngine"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.GridJs.GridAbstractCalculationEngine. Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells"
type: docs
url: /fr/net/aspose.cells.gridjs/gridabstractcalculationengine/
---
## GridAbstractCalculationEngine class

Représente le moteur de calcul personnalisé de l'utilisateur pour étendre le moteur de calcul par défaut d'Aspose.Cells.

```csharp
public abstract class GridAbstractCalculationEngine
```

## Méthodes

| Nom | Description |
| --- | --- |
| abstract [Calculate](../../aspose.cells.gridjs/gridabstractcalculationengine/calculate/)(GridCalculationData) | Calcule une fonction avec les données fournies. |

### Remarques

L'utilisateur ne doit pas modifier directement aucune partie du Workbook dans cette implémentation (excepté le résultat calculé de la fonction personnalisée, qui peut être défini via la propriété GridCalculationData.CalculatedValue). Sinon, des résultats inattendus ou une Exception peuvent survenir. Si l'utilisateur doit modifier d'autres données que le résultat calculé dans l'implémentation pour certaines fonctions personnalisées, par exemple modifier la formule d'une cellule, le style, etc., il doit rassembler ces données dans cette implémentation et les modifier en dehors du périmètre du calcul de formule.

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

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


