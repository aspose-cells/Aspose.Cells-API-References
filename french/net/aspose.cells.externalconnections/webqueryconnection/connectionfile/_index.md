---
title: "WebQueryConnection.ConnectionFile"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebQueryConnection. Obtient le fichier de connexion"
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/connectionfile/
---
## WebQueryConnection.ConnectionFile property

Obtient le fichier de connexion.

```csharp
public override string ConnectionFile { get; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyConnectionFileDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Créez une feuille de calcul d'exemple avec les données de requête Web
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Web Query Data";
                
                // Obtenez la première connexion de requête Web existante (le cas échéant)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Affichez la valeur de ConnectionFile (propriété en lecture seule)
                    Console.WriteLine("ConnectionFile value: " + connection.ConnectionFile);
                    
                    // Enregistrez le classeur
                    workbook.Save("WebQueryConnectionFileDemo.xlsx");
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


