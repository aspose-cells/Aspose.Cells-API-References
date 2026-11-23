---
title: "SaveOptions.SortExternalNames"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SaveOptions. Indique si le tri des noms définis externes doit être effectué avant l'enregistrement du fichier"
type: docs
url: /fr/net/aspose.cells/saveoptions/sortexternalnames/
---
## SaveOptions.SortExternalNames property

Indique si le tri des noms définis externes doit être effectué avant d'enregistrer le fichier.

```csharp
public bool SortExternalNames { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SaveOptionsPropertySortExternalNamesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Créer une feuille de calcul d’exemple
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données pour rendre l’exemple significatif
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Créer une instance OoxmlSaveOptions qui hérite de SaveOptions
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // Afficher la valeur par défaut de la propriété SortExternalNames
                Console.WriteLine("Default SortExternalNames value: " + saveOptions.SortExternalNames);

                // Définir SortExternalNames sur true
                saveOptions.SortExternalNames = true;
                Console.WriteLine("SortExternalNames set to: " + saveOptions.SortExternalNames);

                // Enregistrez le classeur avec les options d'enregistrement spécifiées
                workbook.Save("SortExternalNamesDemo.xlsx", saveOptions);

                Console.WriteLine("Workbook saved with SortExternalNames enabled.");
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

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


