---
title: "WebQueryConnection.IsTextDates"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WebQueryConnection propriété. Drapeau indiquant si les dates doivent être importées dans les cellules de la feuille de calcul en tant que texte plutôt qu'en tant que dates"
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/istextdates/
---
## WebQueryConnection.IsTextDates property

Indicateur indiquant si les dates doivent être importées dans les cellules de la feuille de calcul en tant que texte plutôt qu'en tant que dates.

```csharp
public bool IsTextDates { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsTextDatesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accéder à la première feuille de calcul
                Worksheet worksheet = workbook.Worksheets[0];
                
                // Créez une connexion de requête Web en chargeant à partir d'un fichier existant
                // ou en accédant à une connexion existante
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Affichez la valeur initiale de IsTextDates
                    Console.WriteLine("Initial IsTextDates value: " + connection.IsTextDates);
                    
                    // Définissez IsTextDates sur true
                    connection.IsTextDates = true;
                    Console.WriteLine("Updated IsTextDates value: " + connection.IsTextDates);
                    
                    // Redéfinissez IsTextDates sur false
                    connection.IsTextDates = false;
                    Console.WriteLine("Final IsTextDates value: " + connection.IsTextDates);
                    
                    // Enregistrer le classeur avec la connexion de requête Web
                    workbook.Save("WebQueryConnectionIsTextDatesDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
                }
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

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


