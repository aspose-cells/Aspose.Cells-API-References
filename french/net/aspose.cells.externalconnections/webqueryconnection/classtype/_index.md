---
title: "WebQueryConnection.ClassType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WebQueryConnection propriété. Obtient le type de cet objet ExternalConnection"
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/classtype/
---
## WebQueryConnection.ClassType property

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

    public class WebQueryConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accéder à une connexion de requête Web existante ou en créer une via une initialisation appropriée
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Afficher la valeur de ClassType (propriété en lecture seule)
                    Console.WriteLine("WebQueryConnection ClassType: " + connection.ClassType);
                    
                    // Vérifiez la valeur d'énumération attendue pour la requête Web
                    Console.WriteLine("Expected WebQuery enum value: " + 
                        (connection.ClassType == ExternalConnectionClassType.WebQuery ? "Match" : "Mismatch"));
                    
                    // Enregistrez le classeur
                    workbook.Save("WebQueryConnectionClassTypeDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
                }
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
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


