---
title: "DataModelConnection.ConnectionString"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataModelConnection. La chaîne d'informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC"
type: docs
url: /fr/net/aspose.cells.externalconnections/datamodelconnection/connectionstring/
---
## DataModelConnection.ConnectionString property

La chaîne d’informations de connexion est utilisée pour établir le contact avec une source de données OLE DB ou ODBC.

```csharp
public override string ConnectionString { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyConnectionStringDemo
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

                // Afficher la valeur initiale de ConnectionString (vide)
                Console.WriteLine("Initial ConnectionString: " + connection.ConnectionString);

                // Définir la propriété ConnectionString
                connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";
                
                // Afficher la valeur mise à jour de ConnectionString
                Console.WriteLine("Updated ConnectionString: " + connection.ConnectionString);

                // Définir les autres propriétés requises pour une connexion complète
                connection.Command = "SELECT * FROM Customers";
                connection.CommandType = OLEDBCommandType.SqlStatement;

                // Enregistrer le classeur avec la connexion
                workbook.Save("ConnectionStringDemo.xlsx");
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


