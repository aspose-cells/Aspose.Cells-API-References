---
title: "CopyOptions.ReferToSheetWithSameName"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CopyOptions. Dans MS Excel, lors de la copie de formules qui font référence à d'autres feuilles de calcul tout en copiant une feuille vers une autre, les formules copiées doivent faire référence au classeur source. Cependant, dans certaines situations, l'utilisateur peut avoir besoin que les formules copiées fassent référence à des feuilles portant le même nom dans le même classeur, par exemple lorsque ces feuilles ont déjà été copiées avant cette opération de copie ; dans ce cas, cette propriété doit rester à true."
type: docs
url: /fr/net/aspose.cells/copyoptions/refertosheetwithsamename/
---
## CopyOptions.ReferToSheetWithSameName property

Dans MS Excel, lors de la copie de formules qui font référence à d'autres feuilles de calcul tout en copiant une feuille vers une autre, les formules copiées doivent faire référence au classeur source. Cependant, dans certaines situations l'utilisateur peut avoir besoin que les formules copiées fassent référence à des feuilles de calcul portant le même nom dans le même classeur, par exemple lorsque ces feuilles ont déjà été copiées avant cette opération de copie, alors cette propriété doit rester à true.

```csharp
public bool ReferToSheetWithSameName { get; set; }
```

### Remarques

La valeur par défaut est true.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CopyOptionsPropertyReferToSheetWithSameNameDemo
    {
        public static void Run()
        {
            // Créer un classeur modèle avec des données d'exemple
            Workbook templateWorkbook = new Workbook();
            Worksheet templateSheet1 = templateWorkbook.Worksheets[0];
            templateSheet1.Name = "Data";
            templateSheet1.Cells["A1"].PutValue("Value");
            templateSheet1.Cells["A2"].PutValue(10);
            templateSheet1.Cells["A3"].PutValue(20);
            
            Worksheet templateSheet2 = templateWorkbook.Worksheets.Add("Summary");
            templateSheet2.Cells["B2"].Formula = "=SUM(Data!A2:A3)";

            // Créer le classeur de sortie
            Workbook outputWorkbook = new Workbook();
            outputWorkbook.Worksheets.Clear();

            // Copier les feuilles de calcul avec ReferToSheetWithSameName activé
            foreach (Worksheet sheet in templateWorkbook.Worksheets)
            {
                outputWorkbook.Worksheets.Add(sheet.Name);
                CopyOptions options = new CopyOptions();
                options.ReferToSheetWithSameName = true;
                outputWorkbook.Worksheets[sheet.Name].Copy(sheet, options);
            }

            // Vérifier que la formule fait référence à la bonne feuille
            Console.WriteLine("Formula in output workbook: " + 
                outputWorkbook.Worksheets["Summary"].Cells["B2"].Formula);
        }
    }
}
```

### Voir aussi

* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


