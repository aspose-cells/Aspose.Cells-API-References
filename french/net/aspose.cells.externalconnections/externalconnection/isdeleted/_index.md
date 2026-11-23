---
title: "ExternalConnection.IsDeleted"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Indique si la connexion du classeur associée a été supprimée. true si la connexion a été supprimée, sinon false"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/isdeleted/
---
## ExternalConnection.IsDeleted property

Indique si la connexion de classeur associée a été supprimée. true si la connexion a été supprimée ; sinon false.

```csharp
public bool IsDeleted { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyIsDeletedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion externe (en supposant qu’elle existe)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Afficher la valeur initiale de IsDeleted
                Console.WriteLine("Initial IsDeleted value: " + connection.IsDeleted);
                
                // Basculer la valeur de IsDeleted (puisqu’elle est en lecture‑écriture)
                connection.IsDeleted = !connection.IsDeleted;
                Console.WriteLine("Updated IsDeleted value: " + connection.IsDeleted);
                
                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("IsDeletedDemo.xlsx");
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


