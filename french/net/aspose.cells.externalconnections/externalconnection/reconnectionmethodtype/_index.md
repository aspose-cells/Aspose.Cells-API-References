---
title: "ExternalConnection.ReconnectionMethodType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Spécifie ce que l’application de feuille de calcul doit faire lorsqu’une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/reconnectionmethodtype/
---
## ExternalConnection.ReconnectionMethodType property

Spécifie ce que l’application de feuille de calcul doit faire lorsqu’une connexion échoue. La valeur par défaut est ReConnectionMethodType.Required.

```csharp
public ReConnectionMethodType ReconnectionMethodType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyReconnectionMethodTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion externe (en supposant qu’elle existe)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Afficher la valeur actuelle de ReconnectionMethodType
                Console.WriteLine("Initial ReconnectionMethodType: " + connection.ReconnectionMethodType);
                
                // Démontrez la définition de la propriété (car elle est en lecture‑écriture)
                connection.ReconnectionMethodType = ReConnectionMethodType.Always;
                Console.WriteLine("Updated ReconnectionMethodType: " + connection.ReconnectionMethodType);
                
                // Parcourir les valeurs possibles pour démontrer la capacité de réglage
                foreach (ReConnectionMethodType method in Enum.GetValues(typeof(ReConnectionMethodType)))
                {
                    connection.ReconnectionMethodType = method;
                    Console.WriteLine($"ReconnectionMethodType set to: {method}");
                }
                
                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("ReconnectionMethodTypeDemo.xlsx");
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

* enum [ReConnectionMethodType](../../reconnectionmethodtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


