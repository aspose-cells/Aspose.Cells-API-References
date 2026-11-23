---
title: "ExternalConnection.ConnectionString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. La chaîne d’informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/connectionstring/
---
## ExternalConnection.ConnectionString property

La chaîne d’informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC.

```csharp
public virtual string ConnectionString { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyConnectionStringDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Créer des données d'exemple
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);
            
            // Créer un tableau croisé dynamique
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Obtenir les connexions de données
            ExternalConnection[] connections = pivotTable.GetSourceDataConnections();
            
            // Afficher la chaîne de connexion si elle existe
            if (connections.Length > 0)
            {
                Console.WriteLine("Connection String: " + connections[0].ConnectionString);
            }
            
            // Enregistrez le classeur
            workbook.Save("PivotTableWithConnection.xlsx");
        }
    }
}
```

### Voir aussi

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


