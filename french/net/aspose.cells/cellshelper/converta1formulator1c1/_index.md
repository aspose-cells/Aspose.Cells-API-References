---
title: "CellsHelper.ConvertA1FormulaToR1C1"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Convertit la formule A1 de la cellule en formule r1c1"
type: docs
url: /fr/net/aspose.cells/cellshelper/converta1formulator1c1/
---
## CellsHelper.ConvertA1FormulaToR1C1 method

Convertit la formule A1 de la cellule en formule r1c1.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertA1FormulaToR1C1(string formula, int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| formule | String | La formule A1. |
| ligne | Int32 | L'index de ligne de la cellule. |
| column | Int32 | L'index de colonne de la cellule. |

### Valeur de retour

La formule R1C1.

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Worksheet.ConvertFormulaReferenceStyle(). Cette propriété sera supprimée 12 mois plus tard, à compter d'août 2023. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodConvertA1FormulaToR1C1WithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Convertir la formule de style A1 en style R1C1
            string r1c1Formula = CellsHelper.ConvertA1FormulaToR1C1("=A1+B2", 0, 0);
            Console.WriteLine("R1C1 Formula: " + r1c1Formula);
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


