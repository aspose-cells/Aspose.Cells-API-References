---
title: "DifLoadOptions.DifLoadOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Constructeur DifLoadOptions. Les options"
type: docs
url: /fr/net/aspose.cells.loading/difloadoptions/difloadoptions/
---
## DifLoadOptions constructor

Les options.

```csharp
public DifLoadOptions()
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;
    using System;

    public class DifLoadOptionsMethodCtorDemo
    {
        public static void Run()
        {
            try
            {
                // Créer une nouvelle instance de DifLoadOptions en utilisant le constructeur sans paramètres
                DifLoadOptions loadOptions = new DifLoadOptions();

                // Créer un nouveau classeur avec les options par défaut
                Workbook workbook = new Workbook();

                // Accéder à la première feuille de calcul
                Worksheet worksheet = workbook.Worksheets[0];

                // Ajouter des données d'exemple pour démontrer que le classeur fonctionne
                worksheet.Cells["A1"].PutValue("DifLoadOptions Constructor Demo");
                worksheet.Cells["A2"].PutValue("Created at: " + DateTime.Now.ToString());
                worksheet.Cells["A4"].PutValue("This demonstrates using the parameterless constructor");

                // Enregistrer le classeur au format DIF
                workbook.Save("DifLoadOptionsCtorDemo.dif", SaveFormat.Dif);

                // Chargez maintenant le fichier DIF enregistré avec DifLoadOptions
                DifLoadOptions difOptions = new DifLoadOptions();
                Workbook loadedWorkbook = new Workbook("DifLoadOptionsCtorDemo.dif", difOptions);

                // Enregistrer les données chargées au format XLSX pour vérification
                loadedWorkbook.Save("DifLoadOptionsCtorVerification.xlsx", SaveFormat.Xlsx);

                Console.WriteLine("DifLoadOptions constructor demo completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DifLoadOptions constructor demo: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [DifLoadOptions](../)
* namespace [Aspose.Cells.Loading](../../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../../)


