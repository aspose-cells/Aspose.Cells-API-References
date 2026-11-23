---
title: "Classe AbstractLowCodeSaveOptionsProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.LowCode.AbstractLowCodeSaveOptionsProvider. Implémentation permettant de fournir plusieurs options d'enregistrement pour les processus nécessitant plusieurs sorties. Par exemple, la fonctionnalité SpreadsheetSplitter nécessite plusieurs destinations pour enregistrer les fichiers découpés."
type: docs
url: /fr/net/aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/
---
## AbstractLowCodeSaveOptionsProvider class

Implémentation permettant de fournir plusieurs options d'enregistrement pour les processus nécessitant plusieurs sorties. Par exemple, la fonctionnalité [`SpreadsheetSplitter`](../spreadsheetsplitter/) nécessite plusieurs destinations pour enregistrer les fichiers découpés.

```csharp
public abstract class AbstractLowCodeSaveOptionsProvider
```

## Méthodes

| Nom | Description |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Libère les ressources après le traitement de la partie découpée actuelle. |
| abstract [GetSaveOptions](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/)(SplitPartInfo) | Obtient les options d'enregistrement à partir desquelles récupérer les paramètres de sortie pour la partie découpée actuelle. Retourner null indique d'ignorer la partie donnée. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeSaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Créez un fournisseur personnalisé en étendant AbstractLowCodeSaveOptionsProvider
            var customProvider = new CustomSaveOptionsProvider();

            // Créez un classeur et une feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplissez quelques données
            worksheet.Cells["A1"].PutValue("Test Data");
            
            // Créez les informations de la partie découpée - dans une utilisation réelle, cela proviendrait de l'API
            // Comme nous ne pouvons pas le construire directement, nous passerons simplement null à des fins de démonstration
            SplitPartInfo splitPartInfo = null;
            
            // Obtenez les options d'enregistrement du fournisseur
            LowCodeSaveOptions saveOptions = customProvider.GetSaveOptions(splitPartInfo);
            
            // Configurez les options d'enregistrement (exemple)
            saveOptions.SaveFormat = SaveFormat.Xlsx;
            
            // Démontrez la finalisation du processus
            customProvider.Finish(saveOptions);
            
            // Enregistrez le classeur (pas directement lié au fournisseur, juste pour la démo)
            workbook.Save("LowCodeSaveOptionsDemo.xlsx");
        }
    }

    // Implémentation personnalisée de AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Créez et renvoyez des options d'enregistrement personnalisées basées sur les informations de la partie
            return new LowCodeSaveOptions()
            {
                SaveFormat = SaveFormat.Xlsx
                // Supprimé CachedFileFolder car il n'existe pas dans LowCodeSaveOptions
            };
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Logique de nettoyage ou de finalisation ici
            Console.WriteLine("Save operation completed for part");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


