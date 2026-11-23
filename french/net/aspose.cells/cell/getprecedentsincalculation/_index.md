---
title: "Cell.GetPrecedentsInCalculation"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Cell. Obtient toutes les références précédentes aux cellules du classeur actuel utilisées par la formule de cette cellule lors de son calcul"
type: docs
url: /fr/net/aspose.cells/cell/getprecedentsincalculation/
---
## Cell.GetPrecedentsInCalculation method

Obtient tous les antécédents (référence aux cellules du classeur actuel) utilisés par la formule de cette cellule lors de son calcul.

```csharp
public IEnumerator GetPrecedentsInCalculation()
```

### Valeur de retour

Énumérateur pour énumérer toutes les références (ReferredArea)

### Remarques

Cette méthode ne peut fonctionner que si la situation suivante est remplie : [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) est vrai pour le classeur et le classeur a été entièrement calculé. Si cette cellule n’est pas une formule ou ne fait référence à aucune autre cellule, null sera renvoyé.

### Exemples

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetPrecedentsInCalculationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            cells["B1"].PutValue(10);
            cells["B2"].PutValue(20);
            cells["A2"].Formula = "=IF(TRUE,B2,B1)";
            
            workbook.Settings.FormulaSettings.EnableCalculationChain = true;
            workbook.CalculateFormula();
            
            IEnumerator en = cells["A2"].GetPrecedentsInCalculation();
            Console.WriteLine("A2's calculation precedents:");
            while(en.MoveNext())
            {
                ReferredArea r = (ReferredArea)en.Current;
                Console.WriteLine(r);
            }
        }
    }
}
```

### Voir aussi

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


