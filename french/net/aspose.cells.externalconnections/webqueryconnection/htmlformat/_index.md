---
title: "WebQueryConnection.HtmlFormat"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WebQueryConnection property. Comment gérer le formatage provenant de la source HTML lors de l'importation des données de requête Web dans la feuille de calcul. Pertinent lorsque sourceData est True"
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/htmlformat/
---
## WebQueryConnection.HtmlFormat property

Comment gérer le formatage provenant de la source HTML lors de l'importation des données de requête Web dans la feuille de calcul. Pertinent lorsque sourceData est True.

```csharp
public HtmlFormatHandlingType HtmlFormat { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyHtmlFormatDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première connexion de requête Web existante (le cas échéant)
            // Ou créer une nouvelle en chargeant un fichier contenant des connexions Web
            if (workbook.DataConnections.Count > 0)
            {
                try
                {
                    WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                    
                    // Afficher la valeur initiale de HtmlFormat
                    Console.WriteLine("Initial HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Définir HtmlFormat sur Rtf (démonstration de l'opération d'écriture)
                    connection.HtmlFormat = HtmlFormatHandlingType.Rtf;
                    Console.WriteLine("Updated HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Définir HtmlFormat sur None
                    connection.HtmlFormat = HtmlFormatHandlingType.None;
                    Console.WriteLine("Final HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Enregistrer le classeur avec la connexion de requête Web
                    workbook.Save("WebQueryConnectionHtmlFormatDemo.xlsx");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error: {ex.Message}");
                }
            }
            else
            {
                Console.WriteLine("No web query connections found in the workbook.");
            }
        }
    }
}
```

### Voir aussi

* enum [HtmlFormatHandlingType](../../htmlformathandlingtype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


