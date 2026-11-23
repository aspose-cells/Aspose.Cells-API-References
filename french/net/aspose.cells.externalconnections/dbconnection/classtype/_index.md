---
title: "DBConnection.ClassType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DBConnection. Obtient le type de cet objet ExternalConnection"
type: docs
url: /fr/net/aspose.cells.externalconnections/dbconnection/classtype/
---
## DBConnection.ClassType property

Obtient le type de cet objet [`ExternalConnection`](../../externalconnection/).

```csharp
public override ExternalConnectionClassType ClassType { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class DBConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Créez une nouvelle instance DBConnection en l’ajoutant à la collection
                // Étant donné que DBConnection n’a pas de constructeur public sans paramètres,
                // nous laisserons la collection le créer pour nous
                var connections = workbook.DataConnections;
                DBConnection dbConnection = (DBConnection)connections[connections.Count];
                
                // Afficher la valeur de ClassType (propriété en lecture seule)
                Console.WriteLine("DBConnection ClassType: " + dbConnection.ClassType);
                
                // Démontrer la définition d’autres propriétés pour rendre l’exemple plus significatif
                dbConnection.ConnectionString = "Server=myServerAddress;Database=myDataBase;";
                dbConnection.CommandType = OLEDBCommandType.TableName;
                dbConnection.Command = "Customers";
                
                // Enregistrez le classeur
                workbook.Save("DBConnectionDemo.xlsx");
                
                Console.WriteLine("ClassType demonstration completed successfully.");
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

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DBConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


