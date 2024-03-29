---
title: GetDependents
second_title: Référence de l'API Aspose.Cells pour .NET
description: Obtenir toutes les cellules dont la formule fait directement référence à cette cellule.
type: docs
weight: 380
url: /fr/net/aspose.cells/cell/getdependents/
---
## Cell.GetDependents method

Obtenir toutes les cellules dont la formule fait directement référence à cette cellule.

```csharp
public Cell[] GetDependents(bool isAll)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| isAll | Boolean | Indique si vérifier les formules dans d'autres feuilles de calcul |

### Remarques

Si une référence contenant cette cellule apparaît dans la formule d'une cellule, cette cellule sera considérée comme la personne à charge de cette cellule, peu importe la référence ou cette cellule est utilisée ou non lors du calcul. Par exemple, bien que la cellule A2 dans la formule "=IF (TRUE,A1,A2)" n'est pas utilisé lors du calcul, cette formule est toujours considérée comme dépendante de A2.  Pour obtenir les formules dont les résultats calculés dépendent de cette cellule, veuillez utiliser[`GetDependentsInCalculation`](../getdependentsincalculation). Lors du traçage des personnes à charge pour une cellule, toutes les formules du classeur ou de la feuille de calcul seront analysées et vérifiées. Il s'agit donc d'un processus chronophage. Si l'utilisateur a besoin de suivre les personnes à charge pour de nombreuses cellules, l'utilisation de cette méthode entraînera de mauvaises performances. Pour des raisons de performances, l'utilisateur doit utiliser[`GetDependentsInCalculation`](../getdependentsincalculation) à la place. Ou, l'utilisateur peut rassembler la carte des précédents de toutes les cellules en[`GetPrecedents`](../getprecedents)tout d'abord, puis construisez la carte des dépendances en fonction de la carte des précédents.

### Exemples

```csharp
[C#]

Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2";
cells["A2"].Formula = "=IF(TRUE,B2,B1)";
Cell[] dependents = cells["B1"].GetDependents(true);
for (int i = 0; i < dependents.Length; i++)
{
     Console.WriteLine(dependents[i].Name);
}
```

### Voir également

* class [Cell](../../cell)
* espace de noms [Aspose.Cells](../../cell)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
