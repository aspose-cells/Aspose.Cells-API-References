---
title: "ExternalConnection.OnlyUseConnectionFile"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ExternalConnection. Indique si l'application de feuille de calcul doit toujours et uniquement utiliser les informations de connexion dans le fichier de connexion externe indiqué par l'attribut odcFile lorsque la connexion est rafraîchie. Si faux, alors l'application de feuille de calcul doit suivre la procédure indiquée par l'attribut reconnectionMethod"
type: docs
url: /fr/net/aspose.cells.externalconnections/externalconnection/onlyuseconnectionfile/
---
## ExternalConnection.OnlyUseConnectionFile property

Indique si l’application de feuille de calcul doit toujours et uniquement utiliser les informations de connexion du fichier de connexion externe indiqué par l’attribut odcFile lors de l’actualisation de la connexion. Si false, alors l’application de feuille de calcul doit suivre la procédure indiquée par l’attribut reconnectionMethod.

```csharp
public bool OnlyUseConnectionFile { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertyOnlyUseConnectionFileDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            try
            {
                // Accédez à la première connexion externe (en supposant qu’elle existe)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Afficher la valeur actuelle de OnlyUseConnectionFile
                Console.WriteLine("Initial OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Définir une nouvelle valeur pour OnlyUseConnectionFile (car c'est en lecture-écriture)
                connection.OnlyUseConnectionFile = true;
                Console.WriteLine("Updated OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Basculer la valeur pour démontrer la capacité de réglage
                connection.OnlyUseConnectionFile = !connection.OnlyUseConnectionFile;
                Console.WriteLine("Toggled OnlyUseConnectionFile value: " + connection.OnlyUseConnectionFile);
                
                // Enregistrez le classeur avec les paramètres de connexion modifiés
                workbook.Save("OnlyUseConnectionFileDemo.xlsx");
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


