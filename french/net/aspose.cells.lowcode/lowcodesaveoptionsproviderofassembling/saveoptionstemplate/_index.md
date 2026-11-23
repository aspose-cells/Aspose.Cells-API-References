---
title: "LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "LowCodeSaveOptionsProviderOfAssembling property. Le modèle pour créer une instance d'options d'enregistrement dans GetSaveOptions"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/
---
## LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate property

Le modèle pour créer une instance d'options d'enregistrement dans [`GetSaveOptions`](../getsaveoptions/).

```csharp
public LowCodeSaveOptions SaveOptionsTemplate { get; set; }
```

### Remarques

Si le modèle a été spécifié, alors l'instance créée copiera tous les paramètres depuis celui-ci et mettra à jour le fichier de sortie en conséquence.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Saving;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySaveOptionsTemplateDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec deux feuilles de calcul
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            Worksheet worksheet1 = workbook.Worksheets[0];
            Worksheet worksheet2 = workbook.Worksheets[1];
            worksheet1.Cells["A1"].PutValue("Sheet1 Content");
            worksheet2.Cells["A1"].PutValue("Sheet2 Content");

            // Créer une instance de LowCodeSaveOptionsProviderOfAssembling
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "Output/Sheet",
                PathTail = ".xlsx",
                BuildPathWithSheetAlways = true,
                UseSheetName = false
            };

            // Afficher l'état initial de SaveOptionsTemplate
            Console.WriteLine("Initial SaveOptionsTemplate is " + (provider.SaveOptionsTemplate == null ? "null" : "set"));

            // Configurer SaveOptionsTemplate avec chiffrement
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();
            Console.WriteLine("SaveOptionsTemplate configured");

            // Créer des options d'enregistrement LowCode
            var saveOptions = new LowCodeSaveOptions();

            // Enregistrer le classeur en utilisant le fournisseur configuré (générera des fichiers séparés par feuille)
            workbook.Save("output_combined.xlsx", saveOptions.SaveFormat);

            Console.WriteLine("Demo executed successfully. Check output files.");
        }
    }
}
```

### Voir aussi

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


