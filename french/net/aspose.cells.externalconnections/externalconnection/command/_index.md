---
title: "ExternalConnection.Command"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/command/
---
## ExternalConnection.Command property

La chaîne contenant la commande de base de données à transmettre à l’API du fournisseur de données qui interagira avec la source externe afin de récupérer les données

```csharp
public virtual string Command { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul et des données d'exemple
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(150);
            
            // Créer une plage de tableau
            var range = worksheet.Cells.CreateRange("A1:B3");
            
            // Créer un tableau croisé dynamique en utilisant la plage comme source
            int index = worksheet.PivotTables.Add("D1", "A1:B3", "PivotTable1");
            var pivotTable = worksheet.PivotTables[index];
            
            // Obtenir les connexions externes
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Afficher la propriété Command de la connexion
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection Command: " + connections[0].Command);
            }
            
            // Enregistrez le classeur
            workbook.Save("ExternalConnectionCommandDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


