---
title: "ExternalConnection.Type"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Obtient ou définit le type de source de données de la connexion externe"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/type/
---
## ExternalConnection.Type property

Obtient ou définit le type DataSource de la connexion externe.

```csharp
[Obsolete("Use ExternalConnection.SourceType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ConnectionDataSourceType Type { get; set; }
```

### Remarques

NOTE: Cette propriété est maintenant obsolète. À la place, veuillez utiliser la propriété ExternalConnection.SourceType. Cette propriété sera supprimée 12 mois plus tard depuis octobre 2024. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion externe (en supposant qu’elle existe)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Afficher la valeur actuelle de Type (opération de lecture)
                Console.WriteLine("Initial Type value: " + connection.Type);
                
                // Définir une nouvelle valeur pour Type (car c'est en lecture-écriture)
                connection.Type = ConnectionDataSourceType.OLEDBBasedSource;
                Console.WriteLine("Updated Type value: " + connection.Type);
                
                // Parcourir les valeurs possibles pour démontrer la capacité de réglage
                foreach (ConnectionDataSourceType type in Enum.GetValues(typeof(ConnectionDataSourceType)))
                {
                    if ((int)type != 102) // Skip duplicate enum value
                    {
                        connection.Type = type;
                        Console.WriteLine($"Type set to: {type}");
                    }
                }
                
                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("TypeDemo.xlsx");
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

* enum [ConnectionDataSourceType](../../connectiondatasourcetype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


