---
title: "ExternalConnection.RefreshInternal"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Spécifie le nombre de minutes entre les rafraîchissements automatiques de la connexion"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/refreshinternal/
---
## ExternalConnection.RefreshInternal property

Spécifie le nombre de minutes entre les rafraîchissements automatiques de la connexion.

```csharp
public int RefreshInternal { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyRefreshInternalDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d’exemple pour rendre l’exemple significatif
            worksheet.Cells["A1"].Value = "Connection Demo";
            
            try
            {
                // Créer une connexion de données (en utilisant la classe de base ExternalConnection)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Définir et afficher la propriété RefreshInternal
                connection.RefreshInternal = 30; // Refresh every 30 minutes
                Console.WriteLine("RefreshInternal value: " + connection.RefreshInternal);
                
                // Modifier l’intervalle de rafraîchissement
                connection.RefreshInternal = 60;
                Console.WriteLine("Updated RefreshInternal value: " + connection.RefreshInternal);
                
                // Enregistrer le classeur avec les paramètres de connexion
                workbook.Save("RefreshInternalDemo.xlsx");
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


