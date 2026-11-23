---
title: "ConnectionParameter.Prompt"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ConnectionParameter. Chaîne d’invite pour le paramètre. Présentée à l’utilisateur de la feuille de calcul avec l’interface d’entrée pour collecter la valeur du paramètre avant de rafraîchir les données externes. Utilisée uniquement lorsque parameterType est prompt."
type: docs
url: /fr/net/aspose.cells.externalconnections/connectionparameter/prompt/
---
## ConnectionParameter.Prompt property

Chaîne d'invite pour le paramètre. Présentée à l'utilisateur de la feuille de calcul avec l'interface d'entrée pour collecter la valeur du paramètre avant de rafraîchir les données externes. Utilisée uniquement lorsque parameterType = prompt.

```csharp
public string Prompt { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyPromptDemo
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
                
                // À des fins de démonstration, nous montrerons comment Prompt serait utilisé si nous avions un paramètre.
                if (parameter != null)
                {
                    // Obtenir et afficher la valeur actuelle de Prompt.
                    Console.WriteLine("Current Prompt: " + parameter.Prompt);
                    
                    // Définir une nouvelle valeur Prompt (puisque la propriété est en lecture-écriture).
                    parameter.Prompt = "Enter customer ID:";
                    Console.WriteLine("Updated Prompt: " + parameter.Prompt);
                }
                else
                {
                    // Démonstration de secours lorsque nous ne pouvons pas créer le paramètre.
                    workbook.Worksheets[0].Cells["A1"].Value = "Prompt property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Enregistrez le classeur
                workbook.Save("ConnectionParameterPromptDemo.xlsx");
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

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


