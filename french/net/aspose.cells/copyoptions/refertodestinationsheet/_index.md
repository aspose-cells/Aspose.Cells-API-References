---
title: "CopyOptions.ReferToDestinationSheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CopyOptions. Lors de la copie de la plage dans le même fichier et que le graphique fait référence à la feuille source, False signifie que la source de données du graphique copié ne sera pas modifiée. True signifie que la source de données du graphique copié fait référence à la feuille de destination."
type: docs
url: /fr/net/aspose.cells/copyoptions/refertodestinationsheet/
---
## CopyOptions.ReferToDestinationSheet property

Lors de la copie de la plage dans le même fichier et que le graphique fait référence à la feuille source, False signifie que la source de données du graphique copié ne sera pas modifiée. True signifie que la source de données du graphique copié fait référence à la feuille de destination.

```csharp
public bool ReferToDestinationSheet { get; set; }
```

### Remarques

La valeur par défaut est false, cela fonctionne comme MS Excel. Par exemple : si vous copiez un graphique dont la source de données est "sheet1!A1:B10" depuis la feuille de calcul "sheet1" vers une autre feuille "sheet2", la source de données sera modifiée en "sheet2!A1:B10".

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToDestinationSheetDemo
    {
        public static void Run()
        {
            // Créer le classeur source avec des données d'exemple
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B1"].PutValue(100);
            sourceSheet.Cells["A2"].PutValue("=SUM(B1)");

            // Créer le classeur de destination
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets.Add("DestinationSheet");

            // Définir les options de copie avec ReferToDestinationSheet
            CopyOptions copyOptions = new CopyOptions();
            copyOptions.ReferToDestinationSheet = true;

            // Copier la feuille de calcul avec les options
            destSheet.Copy(sourceSheet, copyOptions);

            // Enregistrer le résultat
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


