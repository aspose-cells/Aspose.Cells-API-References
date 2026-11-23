---
title: "Classe CopyOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.CopyOptions. Représente les options de copie"
type: docs
url: /fr/net/aspose.cells/copyoptions/
---
## CopyOptions class

Représente les options de copie.

```csharp
public class CopyOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [CopyOptions](copyoptions/)() | Constructeur CopyOptions. |

## Propriétés

| Nom | Description |
| --- | --- |
| [ColumnCharacterWidth](../../aspose.cells/copyoptions/columncharacterwidth/) { get; set; } | Indique si la largeur des colonnes est copiée en unités de caractères. |
| [CopyInvalidFormulasAsValues](../../aspose.cells/copyoptions/copyinvalidformulasasvalues/) { get; set; } | Si la formule n'est pas valide pour la destination cible, seules les valeurs sont copiées. |
| [CopyNames](../../aspose.cells/copyoptions/copynames/) { get; set; } | Indique si les noms sont copiés. |
| [ExtendToAdjacentRange](../../aspose.cells/copyoptions/extendtoadjacentrange/) { get; set; } | Indique s'il faut étendre les plages lors de la copie de la plage vers la plage adjacente. |
| [KeepMacros](../../aspose.cells/copyoptions/keepmacros/) { get; set; } | Indique s'il faut conserver les macros ; |
| [ReferToDestinationSheet](../../aspose.cells/copyoptions/refertodestinationsheet/) { get; set; } | Lors de la copie de la plage dans le même fichier et que le graphique fait référence à la feuille source, False signifie que la source de données du graphique copié ne sera pas modifiée. True signifie que la source de données du graphique copié fait référence à la feuille de destination. |
| [ReferToSheetWithSameName](../../aspose.cells/copyoptions/refertosheetwithsamename/) { get; set; } | Dans MS Excel, lors de la copie de formules qui font référence à d'autres feuilles de calcul tout en copiant une feuille vers une autre, les formules copiées doivent faire référence au classeur source. Cependant, dans certaines situations l'utilisateur peut avoir besoin que les formules copiées fassent référence à des feuilles de calcul portant le même nom dans le même classeur, par exemple lorsque ces feuilles ont déjà été copiées avant cette opération de copie, alors cette propriété doit rester à true. |
| [UpdateInvalidReferencesToTargetSheet](../../aspose.cells/copyoptions/updateinvalidreferencestotargetsheet/) { get; set; } | Indique s'il faut se référer à la feuille de destination si la feuille référencée n'est pas copiée. |

### Exemples

```csharp
using Aspose.Cells;
using System;

namespace AsposeCellsExamples
{
    public class CopyOptionsDemo
    {
        public static void CopyOptionsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            sheet.Cells["A1"].PutValue("Hello");
            sheet.Cells["A2"].PutValue("World");

            // Créer un nouveau classeur dans lequel copier les données
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Créer un objet CopyOptions
            CopyOptions copyOptions = new CopyOptions
            {
                KeepMacros = true,
                ExtendToAdjacentRange = true,
                CopyNames = true,
                CopyInvalidFormulasAsValues = true,
                ColumnCharacterWidth = true,
                ReferToSheetWithSameName = true,
                ReferToDestinationSheet = true
            };

            // Copier les données de la feuille de calcul source vers la feuille de calcul de destination
            destSheet.Cells.CopyRows(sheet.Cells, 0, 0, 2, copyOptions);

            // Enregistrer le classeur de destination
            destWorkbook.Save("CopyOptionsExample.xlsx");
            destWorkbook.Save("CopyOptionsExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


