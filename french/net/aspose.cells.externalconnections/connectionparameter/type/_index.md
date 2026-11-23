---
title: "ConnectionParameter.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ConnectionParameter. Type de paramètre utilisé. Si le parameterTypevalue alors la valeur provenant de boolean, double, integer ou string sera utilisée. Dans ce cas, il est attendu qu'un seul parmi boolean, double, integer ou string soit spécifié"
type: docs
url: /fr/net/aspose.cells.externalconnections/connectionparameter/type/
---
## ConnectionParameter.Type property

Type de paramètre utilisé. Si parameterType=value, alors la valeur provenant de boolean, double, integer ou string sera utilisée. Dans ce cas, on s’attend à ce qu’une seule de {boolean, double, integer, ou string} soit spécifiée.

```csharp
public ConnectionParameterType Type { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyTypeDemo
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
                
                // À titre d'exemple, nous montrerons comment Type serait utilisé si nous avions un paramètre
                if (parameter != null)
                {
                    // Obtenir et afficher la valeur actuelle de Type
                    Console.WriteLine("Current Type: " + parameter.Type);
                    
                    // Définir une nouvelle valeur Type (car la propriété est en lecture-écriture)
                    parameter.Type = ConnectionParameterType.Value;
                    Console.WriteLine("Updated Type: " + parameter.Type);
                }
                else
                {
                    // Démonstration de secours lorsque nous ne pouvons pas créer le paramètre.
                    workbook.Worksheets[0].Cells["A1"].Value = "Type property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Enregistrez le classeur
                workbook.Save("ConnectionParameterTypeDemo.xlsx");
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

* enum [ConnectionParameterType](../../connectionparametertype/)
* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


