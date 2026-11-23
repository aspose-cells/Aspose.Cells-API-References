---
title: "ExternalConnection.OdcFile"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Spécifie le chemin complet vers le fichier de connexion externe à partir duquel cette connexion a été créée. Si une connexion échoue lors d’une tentative de rafraîchissement des données et reconnectionMethod1, l’application de feuille de calcul réessaiera en utilisant les informations du fichier de connexion externe au lieu de l’objet de connexion intégré au classeur."
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/odcfile/
---
## ExternalConnection.OdcFile property

Spécifie le chemin complet vers le fichier de connexion externe à partir duquel cette connexion a été créée. Si une connexion échoue lors d’une tentative d’actualisation des données, et reconnectionMethod=1, alors l’application de feuille de calcul réessaiera en utilisant les informations du fichier de connexion externe au lieu de l’objet de connexion intégré au classeur.

```csharp
public string OdcFile { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOdcFileDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion externe (en supposant qu’elle existe)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Affichez la valeur actuelle de OdcFile
                Console.WriteLine("Initial OdcFile value: " + connection.OdcFile);
                
                // Définissez une nouvelle valeur pour OdcFile (car elle est en lecture‑écriture)
                connection.OdcFile = @"C:\Connections\ExternalData.odc";
                Console.WriteLine("Updated OdcFile value: " + connection.OdcFile);
                
                // Effacez la valeur de OdcFile
                connection.OdcFile = string.Empty;
                Console.WriteLine("Cleared OdcFile value: " + connection.OdcFile);
                
                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("OdcFileDemo.xlsx");
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


