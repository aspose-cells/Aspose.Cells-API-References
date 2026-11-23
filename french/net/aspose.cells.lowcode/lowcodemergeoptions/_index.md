---
title: "Classe LowCodeMergeOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.LowCodeMergeOptions. Options pour fusionner plusieurs fichiers modèle en un seul"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodemergeoptions/
---
## LowCodeMergeOptions class

Options pour fusionner plusieurs fichiers de modèle en un seul.

```csharp
public class LowCodeMergeOptions
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [LowCodeMergeOptions](lowcodemergeoptions/)() | Le constructeur par défaut. |

## Propriétés

| Nom | Description |
| --- | --- |
| [LoadOptionsProvider](../../aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/) { get; set; } | Fournisseur d'options d'enregistrement pour enregistrer les parties découpées. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodemergeoptions/saveoptions/) { get; set; } | Options d'enregistrement pour enregistrer les parties découpées. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeMergeOptionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créer et configurer LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            
            // Définir les options d’enregistrement pour le format de sortie
            mergeOptions.SaveOptions = new LowCodeSaveOptions();
            
            // Attribuer un fournisseur d’options de chargement personnalisé
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();
            
            // Exemple d’intégration (utilisation hypothétique avec la fonctionnalité de fusion)
            // Cela serait généralement appelé avec des chemins de fichiers réels
            // Workbook.Merge(new string[] { "template1.xlsx", "template2.xlsx" }, mergeOptions);
            
            // Enregistrer le classeur (à des fins de démonstration)
            workbook.Save("LowCodeMergeOptionsDemo.xlsx");
        }
    }

    // Fournisseur personnalisé implémentant la classe abstraite
    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {
        public override bool MoveNext()
        {
            // Implémentation minimale pour satisfaire l’exigence abstraite
            return false;
        }

        public override LowCodeLoadOptions Current
        {
            get { throw new InvalidOperationException(); }
        }

        public LoadOptions GetLoadOptions(string fileName)
        {
            if (fileName.EndsWith(".xlsx", StringComparison.OrdinalIgnoreCase))
            {
                return new LoadOptions(LoadFormat.Xlsx);
            }
            return new LoadOptions();
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


