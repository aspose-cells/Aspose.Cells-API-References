---
title: "WebQueryConnection.IsParsePre"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebQueryConnection. Indicateur indiquant si les données contenues dans les balises HTML PRE de la page Web sont analysées en colonnes lors de l'importation de la page dans une table de requête"
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/isparsepre/
---
## WebQueryConnection.IsParsePre property

Indicateur indiquant si les données contenues dans les balises HTML PRE de la page Web sont analysées en colonnes lors de l'importation de la page dans une table de requête.

```csharp
public bool IsParsePre { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsParsePreDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Créez une nouvelle connexion de requête Web en utilisant la connexion existante du classeur
                WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                
                // Affichez la valeur initiale de IsParsePre (par défaut)
                Console.WriteLine("Initial IsParsePre value: " + connection.IsParsePre);
                
                // Définissez IsParsePre sur true
                connection.IsParsePre = true;
                Console.WriteLine("Updated IsParsePre value: " + connection.IsParsePre);
                
                // Rétablir IsParsePre à false
                connection.IsParsePre = false;
                Console.WriteLine("Final IsParsePre value: " + connection.IsParsePre);
                
                // Enregistrez le classeur
                workbook.Save("WebQueryConnectionIsParsePreDemo.xlsx");
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


