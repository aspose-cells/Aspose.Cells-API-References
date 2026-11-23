---
title: "DataModelConnection.ClassType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataModelConnection. Obtient le type de cet objet ExternalConnection"
type: docs
url: /fr/net/aspose.cells.externalconnections/datamodelconnection/classtype/
---
## DataModelConnection.ClassType property

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
    using Aspose.Cells.QueryTables;
    using System;
    using System.Runtime.Serialization;

    public class DataModelConnectionPropertyClassTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créer une instance de DataModelConnection en utilisant un objet non initialisé
            DataModelConnection connection = (DataModelConnection)FormatterServices.GetUninitializedObject(typeof(DataModelConnection));
            ((IList<ExternalConnection>)workbook.DataConnections).Add(connection);

            // Afficher la valeur actuelle de ClassType (propriété lecture‑seule)
            Console.WriteLine("Current ClassType value: " + connection.ClassType);

            // Configurer les propriétés de connexion
            connection.Command = "SELECT * FROM Products";
            connection.CommandType = OLEDBCommandType.SqlStatement;
            connection.ConnectionString = "Provider=SQLOLEDB;Data Source=Northwind;Integrated Security=SSPI";

            // Démontrer comment ClassType affecte la gestion de la connexion
            if (connection.ClassType == ExternalConnectionClassType.DataModel)
            {
                Console.WriteLine("This is a Data Model connection");
                // Ajouter PowerQueryFormula pour la connexion au modèle de données
                PowerQueryFormulaCollection queries = workbook.DataMashup.PowerQueryFormulas;
                string formulaDef = "let Source = Sql.Database(\"myServer\", \"myDB\") in Source";
                PowerQueryFormula query = (PowerQueryFormula)FormatterServices.GetUninitializedObject(typeof(PowerQueryFormula));
                query.Name = "ProductQuery";
                typeof(PowerQueryFormula).GetProperty("FormulaDefinition").SetValue(query, formulaDef);
                ((IList<PowerQueryFormula>)queries).Add(query);
            }

            // Enregistrez le classeur
            workbook.Save("DataModelConnectionClassTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ExternalConnectionClassType](../../externalconnectionclasstype/)
* class [DataModelConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


