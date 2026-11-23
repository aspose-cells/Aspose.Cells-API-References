---
title: "Workbook.UpdateLinkedDataSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode Workbook. Si ce classeur contient des liens externes vers d’autres sources de données, Aspose.Cells tentera de récupérer les dernières données des sources fournies."
type: docs
url: /fr/net/aspose.cells/workbook/updatelinkeddatasource/
---
## Workbook.UpdateLinkedDataSource method

Si ce classeur contient des liens externes vers d’autres sources de données, Aspose.Cells tentera de récupérer les dernières données des sources fournies.

```csharp
public void UpdateLinkedDataSource(Workbook[] externalWorkbooks)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| externalWorkbooks | Workbook[] | Classeurs qui seront utilisés pour mettre à jour les données des liens externes référencés par ce classeur. La correspondance de ces classeurs avec les liens externes est déterminée par [`FileName`](../filename/) et [`DataSource`](../../externallink/datasource/). Veuillez donc vous assurer que [`FileName`](../filename/) a été spécifié avec la valeur appropriée pour chaque classeur afin qu’ils puissent être liés au lien externe correspondant. |

### Remarques

Si le lien externe correspondant ne peut pas être trouvé pour un classeur, alors ce classeur sera ignoré. Ainsi, lorsque vous définissez ultérieurement une formule avec un nouveau lien externe que vous souhaitez associer au classeur ignoré, le lien ne pourra pas être établi tant que vous n’aurez pas appelé à nouveau cette méthode avec ces classeurs.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodUpdateLinkedDataSourceWithWorkbookDemo
    {
        public static void Run()
        {
            // Créer un classeur principal avec des références externes
            Workbook mainWorkbook = new Workbook();
            Worksheet mainSheet = mainWorkbook.Worksheets[0];
            mainSheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]Sheet1!A1";

            // Créer un classeur externe qui sera lié
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["A1"].Value = "Updated External Value";

            try
            {
                // Appeler UpdateLinkedDataSource avec le tableau de classeurs externes
                mainWorkbook.UpdateLinkedDataSource(new Workbook[] { externalWorkbook });

                // Calculer les formules pour mettre à jour la référence
                mainWorkbook.CalculateFormula();

                // Afficher la valeur mise à jour
                Console.WriteLine("Updated value in main workbook: " + mainSheet.Cells["A1"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UpdateLinkedDataSource method: {ex.Message}");
            }

            // Enregistrer le résultat
            mainWorkbook.Save("UpdateLinkedDataSourceDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


