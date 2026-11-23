---
title: "ExternalConnection.SavePassword"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Vrai si le mot de passe doit être enregistré dans la chaîne de connexion, sinon Faux"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/savepassword/
---
## ExternalConnection.SavePassword property

Vrai si le mot de passe doit être enregistré dans la chaîne de connexion ; sinon, Faux.

```csharp
public bool SavePassword { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySavePasswordDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Accédez à la première connexion externe (en supposant qu’elle existe)
                ExternalConnection connection = workbook.DataConnections[0];

                // Afficher la valeur actuelle de SavePassword
                Console.WriteLine("Initial SavePassword value: " + connection.SavePassword);

                // Démontrez la définition de la propriété (car elle est en lecture‑écriture)
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Updated SavePassword value: " + connection.SavePassword);

                // Basculer la valeur pour démontrer la capacité de réglage
                connection.SavePassword = !connection.SavePassword;
                Console.WriteLine("Toggled SavePassword value: " + connection.SavePassword);

                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("SavePasswordDemo.xlsx");
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


