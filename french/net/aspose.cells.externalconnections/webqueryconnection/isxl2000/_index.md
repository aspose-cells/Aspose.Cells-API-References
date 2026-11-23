---
title: "WebQueryConnection.IsXl2000"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "WebQueryConnection propriété. Ce drapeau existe pour la compatibilité descendante avec d'anciens fichiers de feuille de calcul existants et est défini sur true si cette requête Web a été actualisée dans une application de feuille de calcul plus récente ou égale à Microsoft Excel 2000. C'est un attribut optionnel qui peut être ignoré"
type: docs
url: /fr/net/aspose.cells.externalconnections/webqueryconnection/isxl2000/
---
## WebQueryConnection.IsXl2000 property

Ce drapeau existe pour assurer la compatibilité descendante avec d'anciens fichiers de feuille de calcul, et il est réglé sur true si cette requête Web a été actualisée dans une application de feuille de calcul plus récente ou égale à Microsoft Excel 2000. C'est un attribut optionnel qui peut être ignoré.

```csharp
public bool IsXl2000 { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl2000Demo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            try
            {
                // Accéder à la première connexion de requête Web existante (le cas échéant)
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Affichez la valeur initiale de IsXl2000
                    Console.WriteLine("Initial IsXl2000 value: " + connection.IsXl2000);

                    // Définissez IsXl2000 sur true (car il est en lecture-écriture)
                    connection.IsXl2000 = true;
                    Console.WriteLine("Updated IsXl2000 value: " + connection.IsXl2000);

                    // Redéfinissez IsXl2000 sur false
                    connection.IsXl2000 = false;
                    Console.WriteLine("Final IsXl2000 value: " + connection.IsXl2000);

                    // Enregistrez le classeur
                    workbook.Save("WebQueryConnectionIsXl2000Demo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connection found in the workbook.");
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


