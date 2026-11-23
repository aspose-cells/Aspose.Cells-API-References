---
title: "ExternalConnection.SSOId"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Identifiant pour le Single Sign On (SSO) utilisé pour l’authentification entre un serveur intermédiaire spreadsheetML et la source de données externe"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/ssoid/
---
## ExternalConnection.SSOId property

Identifiant pour Single Sign On (SSO) utilisé pour l'authentification entre un serveur intermédiaire spreadsheetML et la source de données externe.

```csharp
public string SSOId { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySSOIdDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion externe
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Affichez la valeur initiale de SSOId (probablement nulle pour une nouvelle connexion)
                Console.WriteLine("Initial SSOId value: " + connection.SSOId);
                
                // Définissez une nouvelle valeur SSOId (car elle est en lecture‑écriture)
                connection.SSOId = "sso-12345";
                Console.WriteLine("Updated SSOId value: " + connection.SSOId);
                
                // Effacez le SSOId
                connection.SSOId = null;
                Console.WriteLine("Cleared SSOId value: " + connection.SSOId);
                
                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("SSOIdDemo.xlsx");
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


