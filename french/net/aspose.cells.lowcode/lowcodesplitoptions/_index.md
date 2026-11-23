---
title: "Classe LowCodeSplitOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.LowCodeSplitOptions. Options pour diviser le tableur"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesplitoptions/
---
## LowCodeSplitOptions class

Options pour diviser la feuille de calcul.

```csharp
public class LowCodeSplitOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LowCodeSplitOptions](lowcodesplitoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [LoadOptions](../../aspose.cells.lowcode/lowcodesplitoptions/loadoptions/) { get; set; } | Options de chargement pour charger le tableur qui sera divisé. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptions/) { get; set; } | Options d'enregistrement pour enregistrer les parties découpées. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/) { get; set; } | Fournisseur d'options d'enregistrement pour enregistrer les parties découpées. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeSplitOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir la feuille de calcul avec des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample Data for Splitting");
            
            // Créer une instance de LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // Configurer LoadOptions (exemple : gérer une source protégée par mot de passe)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // Configurer SaveOptions (exemple : définir le format de sortie par défaut)
            splitOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Implémenter un fournisseur personnalisé de SaveOptions pour des paramètres de sortie dynamiques
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // Exemple d'intégration : diviser le classeur en parties en utilisant les options configurées
            // (Supposer l'existence d'une méthode comme LowCodeEngine.Split(workbook, splitOptions, "outputDir"))
            // LowCodeEngine.Split(workbook, splitOptions, "OutputDirectory");
            
            // Enregistrer le classeur original à des fins de démonstration
            workbook.Save("LowCodeSplitOptionsDemo.xlsx");
        }

        // Implémentation personnalisée de SaveOptionsProvider
        private class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // Logique d'exemple : alterner les paramètres en fonction de l'index de division
                return new LowCodeSaveOptions();
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


