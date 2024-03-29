---
title: GetDependentsInCalculation
second_title: Référence de l'API Aspose.Cells pour .NET
description: Obtient toutes les cellules dont le résultat calculé dépend de cette cellule.
type: docs
weight: 390
url: /fr/net/aspose.cells/cell/getdependentsincalculation/
---
## Cell.GetDependentsInCalculation method

Obtient toutes les cellules dont le résultat calculé dépend de cette cellule.

```csharp
public IEnumerator GetDependentsInCalculation(bool recursive)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| recursive | Boolean | Si renvoie les personnes à charge qui ne font pas directement référence à cette cellule mais font référence à d'autres feuilles de cette cellule |

### Return_Value

Énumérateur pour énumérer toutes les personnes à charge (objets Cellule)

### Remarques

Pour utiliser cette méthode, assurez-vous que le classeur a été défini avec la valeur true for [`EnableCalculationChain`](../../formulasettings/enablecalculationchain) et a été entièrement calculé avec ce paramètre. S'il n'y a pas de référence de formule à cette cellule, null sera renvoyé.

### Exemples

```csharp
[C#]

Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!B2";
cells["A2"].Formula = "=IF(TRUE,B2,B1)";
workbook.Settings.FormulaSettings.EnableCalculationChain = true;
workbook.CalculateFormula();
IEnumerator en = cells["B1"].GetDependentsInCalculation(false);
Console.WriteLine("B1's calculation dependents:");
while(en.MoveNext())
{
    Cell c = (Cell)en.Current;
    Console.WriteLine(c.Name);
}
en = cells["B2"].GetDependentsInCalculation(false);
Console.WriteLine("B2's calculation dependents:");
while(en.MoveNext())
{
    Cell c = (Cell)en.Current;
    Console.WriteLine(c.Name);
}
```

### Voir également

* class [Cell](../../cell)
* espace de noms [Aspose.Cells](../../cell)
* Assemblée [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
