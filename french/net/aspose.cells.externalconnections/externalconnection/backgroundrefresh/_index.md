---
title: "ExternalConnection.BackgroundRefresh"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Indique si la connexion peut être rafraîchie en arrière‑plan de façon asynchrone. true si l’utilisation préférée de la connexion est de rafraîchir de façon asynchrone en arrière‑plan, false si l’utilisation préférée est de rafraîchir de façon synchrone au premier plan."
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/backgroundrefresh/
---
## ExternalConnection.BackgroundRefresh property

Indique si la connexion peut être actualisée en arrière‑plan (asynchrone). true si l’utilisation préférée de la connexion est de rafraîchir de façon asynchrone en arrière‑plan ; false si l’utilisation préférée est de rafraîchir de façon synchrone au premier plan.

```csharp
public bool BackgroundRefresh { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyBackgroundRefreshDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion externe (en supposant qu’elle existe)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Affichez la valeur actuelle de BackgroundRefresh
                Console.WriteLine("Initial BackgroundRefresh value: " + connection.BackgroundRefresh);
                
                // Basculez la valeur de BackgroundRefresh
                connection.BackgroundRefresh = !connection.BackgroundRefresh;
                Console.WriteLine("Updated BackgroundRefresh value: " + connection.BackgroundRefresh);
                
                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("BackgroundRefreshDemo.xlsx");
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


