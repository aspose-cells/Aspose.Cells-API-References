---
title: "ExternalLink.IsVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalLink. Indique si ce lien externe est visible dans MS Excel"
type: docs
url: /fr/net/aspose.cells/externallink/isvisible/
---
## ExternalLink.IsVisible property

Indique si ce lien externe est visible dans MS Excel.

```csharp
public bool IsVisible { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Créer un classeur avec des liens externes
            Workbook workbook = new Workbook();
            
            // Ajoutez des données à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("External Link Demo");
            
            // Créer un nouveau classeur à utiliser comme source du lien externe
            Workbook externalWorkbook = new Workbook();
            externalWorkbook.Worksheets[0].Cells["A1"].PutValue(100);
            externalWorkbook.Save("external_data.xlsx");
            
            // Ajouter une référence de lien externe
            workbook.Worksheets[0].Cells["B1"].Formula = "='[external_data.xlsx]Sheet1'!A1";
            
            // Vérifier les liens externes (ils seront créés automatiquement lors du chargement des formules)
            foreach (ExternalLink link in workbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link visibility: {link.IsVisible}");
                Console.WriteLine($"External link data source: {link.DataSource}");
            }
            
            // Créer un autre classeur pour démontrer le chargement d'un fichier existant
            Workbook workbook2 = new Workbook();
            workbook2.Worksheets[0].Cells["A1"].PutValue("=SUM([example.xls]Sheet1!A1:A10)");
            
            // Enregistrer et recharger pour démontrer les liens externes
            workbook2.Save("output.xlsx");
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Vérifier les liens externes dans le classeur chargé
            foreach (ExternalLink link in loadedWorkbook.Worksheets.ExternalLinks)
            {
                Console.WriteLine($"External link URL: {link.DataSource}, Visible: {link.IsVisible}");
            }
        }
    }
}
```

### Voir aussi

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


