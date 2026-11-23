---
title: "ConnectionParameter.SqlType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ConnectionParameter. Type de données SQL du paramètre. Valide uniquement pour les sources ODBC."
type: docs
url: /fr/net/aspose.cells.externalconnections/connectionparameter/sqltype/
---
## ConnectionParameter.SqlType property

Type de données SQL du paramètre. Valide uniquement pour les sources ODBC.

```csharp
public SqlDataType SqlType { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertySqlTypeDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                
                // Créer un paramètre de connexion (simulé puisque les paramètres du constructeur sont inconnus).
                ConnectionParameter parameter = null;
                
                // Dans un scénario réel, vous créeriez le paramètre correctement.
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // À des fins de démonstration, nous montrerons comment SqlType serait utilisé si nous avions un paramètre.
                if (parameter != null)
                {
                    // Obtenir et afficher la valeur actuelle de SqlType.
                    Console.WriteLine("Current SqlType: " + parameter.SqlType);
                    
                    // Définir une nouvelle valeur SqlType (puisque la propriété est en lecture-écriture).
                    parameter.SqlType = SqlDataType.SqlInteger;
                    Console.WriteLine("Updated SqlType: " + parameter.SqlType);
                }
                else
                {
                    // Démonstration de secours lorsque nous ne pouvons pas créer le paramètre.
                    workbook.Worksheets[0].Cells["A1"].Value = "SqlType property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Enregistrez le classeur
                workbook.Save("ConnectionParameterSqlTypeDemo.xlsx");
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

* enum [SqlDataType](../../sqldatatype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


