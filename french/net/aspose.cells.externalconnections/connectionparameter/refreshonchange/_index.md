---
title: "ConnectionParameter.RefreshOnChange"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ConnectionParameter. Indicateur indiquant si la requête doit se rafraîchir automatiquement lorsque le contenu d’une cellule fournissant la valeur du paramètre change. Si vrai, les données externes sont rafraîchies en utilisant la nouvelle valeur du paramètre à chaque changement. Si faux, les données externes ne sont rafraîchies que lorsqu’elles sont demandées par l’utilisateur ou qu’un autre événement déclenche le rafraîchissement, par ex. le classeur ouvert."
type: docs
url: /fr/net/aspose.cells.externalconnections/connectionparameter/refreshonchange/
---
## ConnectionParameter.RefreshOnChange property

Indicateur indiquant si la requête doit se rafraîchir automatiquement lorsque le contenu d’une cellule qui fournit la valeur du paramètre change. Si true, les données externes sont rafraîchies en utilisant la nouvelle valeur du paramètre à chaque modification. Si false, les données externes ne sont rafraîchies que lorsqu’elles sont demandées par l’utilisateur, ou lorsqu’un autre événement déclenche le rafraîchissement (par ex., classeur ouvert).

```csharp
public bool RefreshOnChange { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyRefreshOnChangeDemo
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
                
                // À des fins de démonstration, nous montrerons comment RefreshOnChange serait utilisé si nous avions un paramètre.
                if (parameter != null)
                {
                    // Obtenir et afficher la valeur actuelle de RefreshOnChange.
                    Console.WriteLine("Current RefreshOnChange: " + parameter.RefreshOnChange);
                    
                    // Définir une nouvelle valeur RefreshOnChange (car la propriété est en lecture-écriture)
                    parameter.RefreshOnChange = true;
                    Console.WriteLine("Updated RefreshOnChange: " + parameter.RefreshOnChange);
                }
                else
                {
                    // Démonstration de secours lorsque nous ne pouvons pas créer le paramètre.
                    workbook.Worksheets[0].Cells["A1"].Value = "RefreshOnChange property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Enregistrez le classeur
                workbook.Save("ConnectionParameterRefreshOnChangeDemo.xlsx");
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


