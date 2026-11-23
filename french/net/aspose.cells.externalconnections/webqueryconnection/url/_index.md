---
title: "WebQueryConnection.Url"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebQueryConnection. URL à utiliser pour actualiser les données externes"
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/url/
---
## WebQueryConnection.Url property

URL à utiliser pour actualiser les données externes.

```csharp
public string Url { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyUrlDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une connexion de requête Web en l'ajoutant à la collection
            // La collection créera probablement et renverra l'objet de connexion
            WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[workbook.DataConnections.Count];

            // Définir l'URL initiale pour la requête Web
            connection.Url = "https://example.com/data.html";
            Console.WriteLine("Initial URL: " + connection.Url);

            // Modifier l'URL vers une source différente
            connection.Url = "https://example.com/updated-data.xml";
            Console.WriteLine("Updated URL: " + connection.Url);

            // Configurer la connexion pour analyser les données XML
            connection.IsXml = true;

            // Actualiser la connexion de données (récupérerait normalement les données depuis l'URL)
            // Remarque : Un accès Web réel nécessiterait une connectivité réseau
            // workbook.RefreshAllConnections();

            // Enregistrer le classeur avec la connexion de requête Web
            workbook.Save("WebQueryConnectionUrlDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


