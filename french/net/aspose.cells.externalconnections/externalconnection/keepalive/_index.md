---
title: "ExternalConnection.KeepAlive"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Vrai lorsque l'application de feuille de calcul doit faire des efforts pour maintenir la connexion ouverte. Lorsque faux, l'application doit fermer la connexion après avoir récupéré les informations."
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/keepalive/
---
## ExternalConnection.KeepAlive property

True lorsque l’application de feuille de calcul doit s’efforcer de garder la connexion ouverte. Lorsque false, l’application doit fermer la connexion après avoir récupéré les informations.

```csharp
public bool KeepAlive { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyKeepAliveDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion externe (en supposant qu’elle existe)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Afficher la valeur actuelle de KeepAlive
                Console.WriteLine("Initial KeepAlive value: " + connection.KeepAlive);
                
                // Basculer la valeur de KeepAlive puisqu'elle est en lecture-écriture
                connection.KeepAlive = !connection.KeepAlive;
                Console.WriteLine("Updated KeepAlive value: " + connection.KeepAlive);
                
                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("KeepAliveDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


