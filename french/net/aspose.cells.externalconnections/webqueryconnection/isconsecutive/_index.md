---
title: "WebQueryConnection.IsConsecutive"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebQueryConnection. Indicateur indiquant si les délimiteurs consécutifs doivent être traités comme un seul délimiteur"
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/isconsecutive/
---
## WebQueryConnection.IsConsecutive property

Indicateur indiquant si les délimiteurs consécutifs doivent être traités comme un seul délimiteur.

```csharp
public bool IsConsecutive { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsConsecutiveDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Créez une connexion de requête Web en accédant à la première connexion
            // (en supposant qu'au moins une connexion soit disponible)
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
            
            try
            {
                // Affichez la valeur initiale de IsConsecutive (par défaut)
                Console.WriteLine("Initial IsConsecutive value: " + connection.IsConsecutive);
                
                // Définissez IsConsecutive sur true
                connection.IsConsecutive = true;
                Console.WriteLine("Updated IsConsecutive value: " + connection.IsConsecutive);
                
                // Redéfinissez IsConsecutive sur false
                connection.IsConsecutive = false;
                Console.WriteLine("Final IsConsecutive value: " + connection.IsConsecutive);
                
                // Enregistrer le classeur avec la connexion de requête Web
                workbook.Save("WebQueryConnectionIsConsecutiveDemo.xlsx");
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


