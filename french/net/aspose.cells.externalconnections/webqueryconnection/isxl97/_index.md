---
title: "WebQueryConnection.IsXl97"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WebQueryConnection propriété. Ce drapeau existe pour la compatibilité descendante avec d'anciens fichiers de feuille de calcul existants et est défini sur true si cette requête Web a été créée dans Microsoft Excel 97. C'est un attribut optionnel qui peut être ignoré"
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/isxl97/
---
## WebQueryConnection.IsXl97 property

Ce drapeau existe pour assurer la compatibilité descendante avec d'anciens fichiers de feuille de calcul, et il est réglé sur true si cette requête Web a été créée dans Microsoft Excel 97. C'est un attribut optionnel qui peut être ignoré.

```csharp
public bool IsXl97 { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl97Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Créez une feuille de calcul avec quelques données pour rendre l'exemple significatif
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Data";
                
                // Créez une connexion de requête Web en chargeant à partir d'un fichier existant ou en la créant correctement
                // Comme nous ne pouvons pas créer WebQueryConnection directement, nous accéderons à une existante
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Affichez la valeur initiale de IsXl97
                    Console.WriteLine("Initial IsXl97 value: " + connection.IsXl97);
                    
                    // Définissez IsXl97 sur true (car il est en lecture-écriture)
                    connection.IsXl97 = true;
                    Console.WriteLine("Updated IsXl97 value: " + connection.IsXl97);
                    
                    // Redéfinissez IsXl97 sur false
                    connection.IsXl97 = false;
                    Console.WriteLine("Final IsXl97 value: " + connection.IsXl97);
                    
                    // Enregistrez le classeur
                    workbook.Save("WebQueryConnectionIsXl97Demo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
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


