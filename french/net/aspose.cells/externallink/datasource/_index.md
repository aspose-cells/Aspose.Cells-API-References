---
title: "ExternalLink.DataSource"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalLink. Représente la source de données du lien externe"
type: docs
url: /fr/net/aspose.cells/externallink/datasource/
---
## ExternalLink.DataSource property

Représente la source de données du lien externe.

```csharp
public string DataSource { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ExternalLinkPropertyDataSourceDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer un lien externe vers un autre classeur
            worksheet.Cells["A1"].Formula = "='[external.xlsx]Sheet1'!A1";
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx");
            
            // Charger le classeur enregistré pour vérifier les liens externes
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            
            // Accéder à la propriété DataSource du lien externe
            if (loadedWorkbook.Worksheets.ExternalLinks.Count > 0)
            {
                string dataSource = loadedWorkbook.Worksheets.ExternalLinks[0].DataSource;
                Console.WriteLine("External link data source: " + dataSource);
            }
        }
    }
}
```

### Voir aussi

* class [ExternalLink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


