---
title: "ExternalConnection.RefreshOnLoad"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Vrai si cette connexion doit être rafraîchie lors de l'ouverture du fichier, sinon faux"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/refreshonload/
---
## ExternalConnection.RefreshOnLoad property

Vrai si cette connexion doit être rafraîchie lors de l'ouverture du fichier ; sinon, faux.

```csharp
public bool RefreshOnLoad { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshOnLoadDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accéder à la première connexion externe (le classeur est fourni avec des connexions par défaut)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Afficher la valeur initiale de RefreshOnLoad
                Console.WriteLine("Initial RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // Démontrez la définition de la propriété (car elle est en lecture‑écriture)
                connection.RefreshOnLoad = !connection.RefreshOnLoad;
                Console.WriteLine("Updated RefreshOnLoad value: " + connection.RefreshOnLoad);
                
                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("RefreshOnLoadDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


