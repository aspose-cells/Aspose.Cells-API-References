---
title: "ExternalConnectionCollection.GetExternalConnectionById"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode ExternalConnectionCollection. Obtient l'élément ExternalConnection avec l'ID spécifié"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnectioncollection/getexternalconnectionbyid/
---
## ExternalConnectionCollection.GetExternalConnectionById method

Obtient l'élément [`ExternalConnection`](../../externalconnection/) avec l'ID spécifié.

```csharp
public ExternalConnection GetExternalConnectionById(int connId)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| connId | Int32 | ID de connexion externe |

### Valeur de retour

L'élément avec l'ID spécifié.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionCollectionMethodGetExternalConnectionByIdWithInt32Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur avec des connexions de données d'exemple
            Workbook workbook = new Workbook();
            
            // Obtenir la collection de connexions externes
            ExternalConnectionCollection dataConns = workbook.DataConnections;

            // Créer et ajouter des connexions en utilisant les méthodes d'API appropriées
            // Remarque : En utilisation réelle, vous obtiendriez généralement les connexions existantes
            // plutôt que de créer de nouvelles de cette manière
            int connectionId1 = 1;
            int connectionId2 = 2;
            
            // Obtenir une connexion spécifique par ID (sera null initialement)
            ExternalConnection specificConn = dataConns.GetExternalConnectionById(connectionId1);
            
            if (specificConn == null)
            {
                Console.WriteLine($"No connection found with ID {connectionId1}");
                // En utilisation réelle, vous travailleriez avec des connexions existantes
                // ou les créer via les méthodes d'API appropriées
            }
            else
            {
                Console.WriteLine($"Found connection: ID={specificConn.ConnectionId}, Name={specificConn.Name}");
                specificConn.Name = "ModifiedConnection";
            }

            // Enregistrez le classeur
            workbook.Save("ExternalConnectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


