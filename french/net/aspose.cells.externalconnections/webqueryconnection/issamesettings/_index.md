---
title: "WebQueryConnection.IsSameSettings"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WebQueryConnection propriété. Drapeau indiquant s'il faut analyser toutes les tables à l'intérieur d'un bloc PRE avec les mêmes paramètres de largeur que la première ligne"
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/issamesettings/
---
## WebQueryConnection.IsSameSettings property

Indicateur indiquant s'il faut analyser toutes les tables à l'intérieur d'un bloc PRE avec les mêmes paramètres de largeur que la première ligne.

```csharp
public bool IsSameSettings { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsSameSettingsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion de requête Web existante si disponible
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Affichez la valeur initiale de IsSameSettings
                    Console.WriteLine("Initial IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Définissez IsSameSettings sur true (car il est en lecture-écriture)
                    connection.IsSameSettings = true;
                    Console.WriteLine("Updated IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Redéfinissez IsSameSettings sur false
                    connection.IsSameSettings = false;
                    Console.WriteLine("Final IsSameSettings value: " + connection.IsSameSettings);
                    
                    // Enregistrez le classeur
                    workbook.Save("WebQueryConnectionIsSameSettingsDemo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
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


