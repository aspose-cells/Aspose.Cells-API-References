---
title: "CellsHelper.ConvertR1C1FormulaToA1"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode CellsHelper. Convertit la formule r1c1 de la cellule en formule A1"
type: docs
url: /fr/net/aspose.cells/cellshelper/convertr1c1formulatoa1/
---
## CellsHelper.ConvertR1C1FormulaToA1 method

Convertit la formule r1c1 de la cellule en formule A1.

```csharp
[Obsolete("Use Worksheet.ConvertFormulaReferenceStyle() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public static string ConvertR1C1FormulaToA1(string r1c1Formula, int row, int column)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| r1c1Formula | String | La formule r1c1. |
| ligne | Int32 | L'index de ligne de la cellule. |
| column | Int32 | L'index de colonne de la cellule. |

### Valeur de retour

La formule A1.

### Remarques

NOTE : Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Worksheet.ConvertFormulaReferenceStyle(). Cette propriété sera supprimée 12 mois plus tard, à compter d'août 2023. Aspose s'excuse pour tout désagrément que vous avez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodConvertR1C1FormulaToA1WithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définir des formules R1C1 dans les cellules
            worksheet.Cells["A1"].R1C1Formula = "=R[1]C";
            worksheet.Cells["B1"].R1C1Formula = "=RC[1]";
            worksheet.Cells["A2"].R1C1Formula = "=R2C3";
            worksheet.Cells["B2"].R1C1Formula = "=R[-1]C[-1]";

            // Convertir les formules R1C1 au format A1
            string a1Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["A1"].R1C1Formula, 0, 0);
            string b1Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["B1"].R1C1Formula, 0, 0);
            string a2Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["A2"].R1C1Formula, 1, 2);
            string b2Converted = CellsHelper.ConvertR1C1FormulaToA1(worksheet.Cells["B2"].R1C1Formula, 1, 1);

            // Afficher les résultats
            Console.WriteLine("A1 R1C1: {0} -> A1: {1}", worksheet.Cells["A1"].R1C1Formula, a1Converted);
            Console.WriteLine("B1 R1C1: {0} -> A1: {1}", worksheet.Cells["B1"].R1C1Formula, b1Converted);
            Console.WriteLine("A2 R1C1: {0} -> A1: {1}", worksheet.Cells["A2"].R1C1Formula, a2Converted);
            Console.WriteLine("B2 R1C1: {0} -> A1: {1}", worksheet.Cells["B2"].R1C1Formula, b2Converted);
        }
    }
}
```

### Voir aussi

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


