---
title: "ConnectionParameter.CellReference"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ConnectionParameter. Référence de cellule indiquant quelle valeur de cellule utiliser pour le paramètre de requête. Utilisée uniquement lorsque parameterType est cell"
type: docs
url: /fr/net/aspose.cells.externalconnections/connectionparameter/cellreference/
---
## ConnectionParameter.CellReference property

Référence de cellule indiquant la valeur de quelle cellule utiliser pour le paramètre de requête. Utilisée uniquement lorsque parameterType est cell.

```csharp
public string CellReference { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyCellReferenceDemo
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
                
                // À titre d'exemple, nous montrerons comment CellReference serait utilisé si nous avions un paramètre
                if (parameter != null)
                {
                    // Obtenir et afficher la valeur actuelle de CellReference
                    Console.WriteLine("Current CellReference: " + parameter.CellReference);
                    
                    // Définir une nouvelle valeur CellReference (car la propriété est en lecture-écriture)
                    parameter.CellReference = "A1";
                    Console.WriteLine("Updated CellReference: " + parameter.CellReference);
                }
                else
                {
                    // Démonstration de secours lorsque nous ne pouvons pas créer le paramètre.
                    workbook.Worksheets[0].Cells["A1"].Value = "CellReference property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Enregistrez le classeur
                workbook.Save("ConnectionParameterCellReferenceDemo.xlsx");
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


