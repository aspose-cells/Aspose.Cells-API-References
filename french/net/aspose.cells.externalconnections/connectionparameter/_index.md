---
title: "Classe ConnectionParameter"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ExternalConnections.ConnectionParameter. Spécifie les propriétés de tous les paramètres utilisés avec les connexions de données externes. Les paramètres sont valides pour les requêtes ODBC et web."
type: docs
url: /fr/net/aspose.cells.externalconnections/connectionparameter/
---
## ConnectionParameter class

Spécifie les propriétés concernant tous les paramètres utilisés avec les connexions de données externes. Les paramètres sont valides pour les requêtes ODBC et Web.

```csharp
public class ConnectionParameter
```

## Propriétés

| Nom | Description |
| --- | --- |
| [CellReference](../../aspose.cells.externalconnections/connectionparameter/cellreference/) { get; set; } | Référence de cellule indiquant la valeur de quelle cellule utiliser pour le paramètre de requête. Utilisée uniquement lorsque parameterType est cell. |
| [Name](../../aspose.cells.externalconnections/connectionparameter/name/) { get; set; } | Le nom du paramètre. |
| [Prompt](../../aspose.cells.externalconnections/connectionparameter/prompt/) { get; set; } | Chaîne d'invite pour le paramètre. Présentée à l'utilisateur de la feuille de calcul avec l'interface d'entrée pour collecter la valeur du paramètre avant de rafraîchir les données externes. Utilisée uniquement lorsque parameterType = prompt. |
| [RefreshOnChange](../../aspose.cells.externalconnections/connectionparameter/refreshonchange/) { get; set; } | Indicateur indiquant si la requête doit se rafraîchir automatiquement lorsque le contenu d’une cellule qui fournit la valeur du paramètre change. Si true, les données externes sont rafraîchies en utilisant la nouvelle valeur du paramètre à chaque modification. Si false, les données externes ne sont rafraîchies que lorsqu’elles sont demandées par l’utilisateur, ou lorsqu’un autre événement déclenche le rafraîchissement (par ex., classeur ouvert). |
| [SqlType](../../aspose.cells.externalconnections/connectionparameter/sqltype/) { get; set; } | Type de données SQL du paramètre. Valide uniquement pour les sources ODBC. |
| [Type](../../aspose.cells.externalconnections/connectionparameter/type/) { get; set; } | Type de paramètre utilisé. Si parameterType=value, alors la valeur provenant de boolean, double, integer ou string sera utilisée. Dans ce cas, on s’attend à ce qu’une seule de {boolean, double, integer, ou string} soit spécifiée. |
| [Value](../../aspose.cells.externalconnections/connectionparameter/value/) { get; set; } | Valeur numérique non entière, valeur entière, valeur chaîne ou valeur booléenne à utiliser comme paramètre de requête. Utilisé uniquement lorsque parameterType est value. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            
            try
            {
                // Créer un paramètre de connexion en utilisant la réflexion puisque le constructeur n’est pas public
                ConnectionParameter parameter = (ConnectionParameter)Activator.CreateInstance(typeof(ConnectionParameter), nonPublic: true);
                
                // Définir les propriétés de base
                parameter.Name = "CustomerID";
                parameter.Type = ConnectionParameterType.Value;
                parameter.Value = "CUST1001";
                parameter.RefreshOnChange = true;
                parameter.Prompt = "Enter Customer ID:";
                
                // Afficher les informations du paramètre
                Console.WriteLine($"Created parameter: {parameter.Name}");
                Console.WriteLine($"Type: {parameter.Type}");
                Console.WriteLine($"Value: {parameter.Value}");
                Console.WriteLine($"Refresh on change: {parameter.RefreshOnChange}");
                Console.WriteLine($"Prompt: {parameter.Prompt}");
                
                // Enregistrez le classeur
                workbook.Save("ConnectionParameterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ConnectionParameter: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


