---
title: "ExternalConnection.IsNew"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Vrai si la connexion n’a pas été actualisée pour la première fois, sinon faux. Cet état peut se produire lorsque l’utilisateur enregistre le fichier avant qu’une requête ne soit terminée"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/isnew/
---
## ExternalConnection.IsNew property

True si la connexion n’a pas encore été actualisée pour la première fois ; sinon false. Cet état peut se produire lorsque l’utilisateur enregistre le fichier avant que la requête ne se termine.

```csharp
public bool IsNew { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsNewDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion externe (les connexions nouvellement créées sont généralement "IsNew")
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Affichez la valeur initiale de IsNew
                Console.WriteLine("Initial IsNew value: " + connection.IsNew);
                
                // Étant donné que IsNew est en lecture‑écriture, démontrez comment le définir
                connection.IsNew = false;
                Console.WriteLine("Updated IsNew value: " + connection.IsNew);
                
                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("IsNewDemo.xlsx");
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


