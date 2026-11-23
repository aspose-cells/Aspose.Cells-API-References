---
title: "WorksheetCollection.IsRefreshAllConnections"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WorksheetCollection. Indique si toutes les connexions sont rafraîchies à l'ouverture du fichier dans MS Excel"
type: docs
url: /fr/net/aspose.cells/worksheetcollection/isrefreshallconnections/
---
## WorksheetCollection.IsRefreshAllConnections property

Indique si toutes les connexions doivent être actualisées à l'ouverture du fichier dans MS Excel.

```csharp
public bool IsRefreshAllConnections { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyIsRefreshAllConnectionsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la collection de feuilles de calcul
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Ajouter quelques feuilles de calcul d'exemple
            worksheets.Add("Sheet1");
            worksheets.Add("Sheet2");
            
            // Définir la propriété IsRefreshAllConnections
            worksheets.IsRefreshAllConnections = true;
            
            // Afficher la valeur actuelle de IsRefreshAllConnections
            Console.WriteLine("IsRefreshAllConnections: " + worksheets.IsRefreshAllConnections);
            
            // Enregistrez le classeur
            workbook.Save("WorksheetCollectionPropertyIsRefreshAllConnectionsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


