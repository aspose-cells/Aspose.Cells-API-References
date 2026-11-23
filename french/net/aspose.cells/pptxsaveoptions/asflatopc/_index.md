---
title: "PptxSaveOptions.AsFlatOpc"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PptxSaveOptions. Indique si l'enregistrement se fait sous forme de fichier OPC plat pouvant être généré par Open XML SDK"
type: docs
url: /fr/net/aspose.cells/pptxsaveoptions/asflatopc/
---
## PptxSaveOptions.AsFlatOpc property

Indique s'il faut enregistrer en tant que fichier opc plat qui peut être généré par Open XML SDK

```csharp
public bool AsFlatOpc { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PptxSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une feuille de calcul d’exemple
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour rendre l’exemple significatif
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Flat OPC Demo";

            try
            {
                // Créer une instance de PptxSaveOptions
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // Afficher la valeur par défaut de AsFlatOpc
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Définir la propriété sur true pour démontrer son utilisation
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Enregistrer le classeur au format PPTX avec l'option activée
                workbook.Save("AsFlatOpcDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with AsFlatOpc enabled");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


