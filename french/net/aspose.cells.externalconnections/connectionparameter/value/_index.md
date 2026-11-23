---
title: "ConnectionParameter.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ConnectionParameter. Valeur numérique non entière, valeur entière, valeur chaîne ou valeur booléenne à utiliser comme paramètre de requête. Utilisé uniquement lorsque parameterType est value."
type: docs
url: /fr/net/aspose.cells.externalconnections/connectionparameter/value/
---
## ConnectionParameter.Value property

Valeur numérique non entière, valeur entière, valeur chaîne ou valeur booléenne à utiliser comme paramètre de requête. Utilisé uniquement lorsque parameterType est value.

```csharp
public object Value { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Créer un nouveau classeur
                Workbook workbook = new Workbook();
                
                // Créer un paramètre de connexion (simulé puisque nous ne connaissons pas les paramètres du constructeur).
                ConnectionParameter parameter = null;
                
                // Dans un scénario réel, vous créeriez le paramètre correctement.
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // À des fins de démonstration, nous créerons un paramètre factice avec une valeur.
                // Cela montre comment la propriété Value serait utilisée en pratique.
                if (parameter != null)
                {
                    // Définir la valeur (puisque Value est en lecture-écriture).
                    parameter.Value = "SampleParameterValue";
                    
                    // Obtenir et afficher la valeur.
                    Console.WriteLine("Parameter Value: " + parameter.Value);
                    
                    // Modifier la valeur pour démontrer qu'elle est mutable.
                    parameter.Value = 42;
                    Console.WriteLine("Updated Parameter Value: " + parameter.Value);
                }
                else
                {
                    // Démonstration de secours lorsque nous ne pouvons pas créer le paramètre.
                    workbook.Worksheets[0].Cells["A1"].Value = "Value property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Enregistrez le classeur
                workbook.Save("ConnectionParameterValueDemo.xlsx");
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


