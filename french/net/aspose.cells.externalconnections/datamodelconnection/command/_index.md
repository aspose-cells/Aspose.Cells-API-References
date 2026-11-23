---
title: "DataModelConnection.Command"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataModelConnection. La chaîne contenant la commande de base de données à transmettre à l'API du fournisseur de données qui interagira avec la source externe afin de récupérer les données"
type: docs
url: /fr/net/aspose.cells.externalconnections/datamodelconnection/command/
---
## DataModelConnection.Command property

La chaîne contenant la commande de base de données à transmettre à l’API du fournisseur de données qui interagira avec la source externe afin de récupérer les données

```csharp
public override string Command { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyCommandDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Créer une instance de DataModelConnection en utilisant un objet non initialisé
                DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
                ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

                // Afficher la valeur initiale de Command (vide)
                Console.WriteLine("Initial Command: " + connection.Command);

                // Définir la propriété Command
                connection.Command = "SELECT * FROM Customers";
                
                // Afficher la valeur mise à jour de Command
                Console.WriteLine("Updated Command: " + connection.Command);

                // Définir les autres propriétés requises pour une connexion complète
                connection.CommandType = OLEDBCommandType.SqlStatement;
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

                // Enregistrer le classeur avec la connexion
                workbook.Save("CommandDemo.xlsx");
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

* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


