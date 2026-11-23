---
title: "ExternalConnection.Parameters"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Obtient ConnectionParameterCollection pour une requête ODBC ou Web"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/parameters/
---
## ExternalConnection.Parameters property

Obtient [`ConnectionParameterCollection`](../../connectionparametercollection/) pour une requête ODBC ou Web.

```csharp
public ConnectionParameterCollection Parameters { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyParametersDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion externe (en supposant qu’elle existe)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Afficher les informations de la collection Parameters
                ConnectionParameterCollection parameters = connection.Parameters;
                Console.WriteLine($"Number of parameters: {parameters.Count}");
                
                // Afficher les informations de chaque paramètre si disponibles
                foreach (ConnectionParameter param in parameters)
                {
                    Console.WriteLine($"Parameter name: {param.Name}");
                    Console.WriteLine($"Parameter type: {param.Type}");
                    Console.WriteLine($"Parameter prompt: {param.Prompt}");
                    Console.WriteLine("----------------------");
                }
                
                // Enregistrez le classeur
                workbook.Save("ParametersDemo.xlsx");
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

* class [ConnectionParameterCollection](../../connectionparametercollection/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


