---
title: "Classe QueryTable"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.QueryTable. Représente les informations de QueryTable"
type: docs
url: /fr/net/aspose.cells/querytable/
---
## QueryTable class

Représente les informations de QueryTable.

```csharp
public class QueryTable
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AdjustColumnWidth](../../aspose.cells/querytable/adjustcolumnwidth/) { get; set; } | Renvoie ou définit AdjustColumnWidth de l'objet. |
| [ConnectionId](../../aspose.cells/querytable/connectionid/) { get; } | Obtient l'identifiant de connexion de la table de requête. |
| [ExternalConnection](../../aspose.cells/querytable/externalconnection/) { get; } | Obtient la connexion externe associée. |
| [Name](../../aspose.cells/querytable/name/) { get; } | Obtient le nom de la querytable. |
| [PreserveFormatting](../../aspose.cells/querytable/preserveformatting/) { get; set; } | Renvoie ou définit PreserveFormatting de l'objet. |
| [ResultRange](../../aspose.cells/querytable/resultrange/) { get; } | Obtient la plage du résultat. |

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassQueryTableDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple pour créer une table de requête (simulation de données externes)
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("John");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Mary");
            
            // Vérifiez s'il existe des tables de requête dans la feuille de calcul
            if (worksheet.QueryTables.Count > 0)
            {
                // Obtenez la première table de requête
                QueryTable qt = worksheet.QueryTables[0];
                
                // Afficher les propriétés du tableau de requête
                Console.WriteLine("Query Table Name: " + qt.Name);
                Console.WriteLine("Connection ID: " + qt.ConnectionId);
                Console.WriteLine("Result Range: " + qt.ResultRange.Address);
                Console.WriteLine("Preserve Formatting: " + qt.PreserveFormatting);
                Console.WriteLine("Adjust Column Width: " + qt.AdjustColumnWidth);
                
                // Modifier certaines propriétés
                qt.PreserveFormatting = true;
                qt.AdjustColumnWidth = false;
            }
            else
            {
                Console.WriteLine("No query tables found in the worksheet.");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


