---
title: "LowCodeSplitOptions.SaveOptionsProvider"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodeSplitOptions. Fournisseur d'options d'enregistrement pour enregistrer les parties découpées"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/
---
## LowCodeSplitOptions.SaveOptionsProvider property

Fournisseur d'options d'enregistrement pour enregistrer les parties découpées.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### Remarques

Si cette propriété est spécifiée, [`SaveOptions`](../saveoptions/) n'a aucun effet car la sortie de chaque partie découpée sera définie par le fournisseur.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Remplir des données d'exemple
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // Créer une instance de LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // Afficher la valeur actuelle de SaveOptionsProvider (null par défaut)
            Console.WriteLine("Current SaveOptionsProvider value: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Créer un SaveOptionsProvider personnalisé
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // Démontrer l'effet de la définition de SaveOptionsProvider
            // Dans un scénario réel, cela serait utilisé lors du fractionnement des fichiers
            Console.WriteLine("After setting SaveOptionsProvider: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // Enregistrer le classeur (bien que le fractionnement ne soit pas démontré ici)
            workbook.Save("PropertySaveOptionsProviderDemo.xlsx");
        }
    }

    // Implémentation personnalisée de AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // Créer des options d'enregistrement personnalisées pour chaque partie découpée
            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            return options;
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // Effectuer tout nettoyage après l'enregistrement de chaque partie
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### Voir aussi

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


