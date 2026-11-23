---
title: "ExternalConnectionCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnectionCollection. Obtient l'élément ExternalConnection à l'index spécifié"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnectioncollection/item/
---
## ExternalConnectionCollection indexer (1 of 2)

Obtient l'élément [`ExternalConnection`](../../externalconnection/) à l'index spécifié.

```csharp
public ExternalConnection this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice à base zéro de l'élément. |

### Valeur de retour

L’élément à l’index spécifié.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Accéder à la collection de connexions externes
                ExternalConnectionCollection connections = workbook.DataConnections;

                // Vérifier s'il existe des connexions
                if (connections.Count > 0)
                {
                    // Démontrer l'accès à un élément par index (opération de lecture)
                    ExternalConnection connection = connections[0];

                    // Afficher les informations de connexion
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                    Console.WriteLine($"Connection ID: {connection.ConnectionId}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }

                // Enregistrez le classeur
                workbook.Save("ExternalConnectionItemDemo.xlsx");
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

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)

---

## ExternalConnectionCollection indexer (2 of 2)

Obtient l'élément [`ExternalConnection`](../../externalconnection/) avec le nom spécifié.

```csharp
public ExternalConnection this[string connectionName] { get; }
```

| Paramètre | Description |
| --- | --- |
| connectionName | le nom de la connexion de données |

### Valeur de retour

L'élément avec le nom spécifié.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accéder à la collection de connexions externes
                ExternalConnectionCollection connections = workbook.DataConnections;
                
                // Ajouter une connexion d'exemple (si nécessaire pour la démonstration)
                // Cela suppose que la collection autorise l'ajout de connexions
                // connections.Add(new ExternalConnection());
                
                // Démontrer l'accès à un élément par nom (opération de lecture)
                // Remarque : Dans un scénario réel, vous auriez besoin de noms de connexion réels
                if (connections.Count > 0)
                {
                    // Obtenir le premier nom de connexion (si disponible)
                    string connectionName = connections[0].Name;
                    
                    // Accéder à la propriété Item
                    ExternalConnection connection = connections[connectionName];
                    
                    // Afficher les informations de connexion
                    Console.WriteLine($"Connection Name: {connection.Name}");
                    Console.WriteLine($"Connection Type: {connection.Type}");
                }
                else
                {
                    Console.WriteLine("No external connections available to demonstrate Item property");
                }
                
                // Enregistrez le classeur
                workbook.Save("ExternalConnectionDemo.xlsx");
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

* class [ExternalConnection](../../externalconnection/)
* class [ExternalConnectionCollection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


