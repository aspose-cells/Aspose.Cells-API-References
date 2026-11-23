---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexOffset"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSaveOptionsProviderOfPlaceHolders. Décalage de l'index des feuilles entre ce qui est utilisé dans le chemin du fichier et sa valeur réelle SheetIndex"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexOffset property

Décalage de l'index de la feuille entre ce qui est utilisé dans le chemin du fichier et sa valeur réelle ([`SheetIndex`](../../splitpartinfo/sheetindex/)).

```csharp
public int SheetIndexOffset { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetIndexOffsetDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec plusieurs feuilles
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // Créer une instance de LowCodeSaveOptionsProviderOfPlaceHolders
            string pathTemplate = "output_{sheet_index}.xlsx";
            var optionsProvider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // Afficher la valeur actuelle de SheetIndexOffset (la valeur par défaut est 0)
            Console.WriteLine("Current SheetIndexOffset value: " + optionsProvider.SheetIndexOffset);

            // Définir SheetIndexOffset à 1 pour décaler les index des feuilles dans les noms de fichiers de sortie
            optionsProvider.SheetIndexOffset = 1;
            Console.WriteLine("New SheetIndexOffset value: " + optionsProvider.SheetIndexOffset);

            // Configurer les options d'enregistrement
            optionsProvider.SaveOptionsTemplate = new LowCodeSaveOptions();
            optionsProvider.SaveOptionsTemplate.SaveFormat = SaveFormat.Xlsx;

            // Démontrer l'effet de SheetIndexOffset sur les noms de fichiers de sortie
            // Normalement, cela serait utilisé avec GetSaveOptions() lors des opérations d'enregistrement réelles
            Console.WriteLine("With SheetIndexOffset=1, output files would be named:");
            Console.WriteLine("Sheet1 -> output_1.xlsx (original index 0 + offset 1)");
            Console.WriteLine("Sheet2 -> output_2.xlsx (original index 1 + offset 1)");
            Console.WriteLine("Sheet3 -> output_3.xlsx (original index 2 + offset 1)");

            // Réinitialiser à la valeur par défaut
            optionsProvider.SheetIndexOffset = 0;
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


