---
title: "ExternalConnection.SaveData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Vrai si les données externes récupérées via la connexion pour remplir un tableau doivent être enregistrées avec le classeur, sinon faux"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/savedata/
---
## ExternalConnection.SaveData property

Vrai si les données externes récupérées via la connexion pour remplir un tableau doivent être enregistrées avec le classeur ; sinon, faux.

```csharp
public bool SaveData { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySaveDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion externe (en supposant qu’elle existe)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Afficher la valeur actuelle de SaveData
                Console.WriteLine("Initial SaveData value: " + connection.SaveData);
                
                // Démontrez la définition de la propriété (car elle est en lecture‑écriture)
                connection.SaveData = !connection.SaveData;
                Console.WriteLine("Updated SaveData value: " + connection.SaveData);
                
                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("SaveDataDemo.xlsx");
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


