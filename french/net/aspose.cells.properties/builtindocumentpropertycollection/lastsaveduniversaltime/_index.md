---
title: "BuiltInDocumentPropertyCollection.LastSavedUniversalTime"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "BuiltInDocumentPropertyCollection property. Obtient ou définit l'heure universelle du dernier enregistrement"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/lastsaveduniversaltime/
---
## BuiltInDocumentPropertyCollection.LastSavedUniversalTime property

Obtient ou définit l'heure universelle de la dernière sauvegarde.

```csharp
public DateTime LastSavedUniversalTime { get; set; }
```

### Remarques

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedUniversalTimeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux propriétés de document intégrées
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Définir la propriété LastSavedUniversalTime
            DateTime utcNow = DateTime.UtcNow;
            builtInProperties.LastSavedUniversalTime = utcNow;

            // Afficher la valeur définie
            Console.WriteLine("LastSavedUniversalTime set to: " + builtInProperties.LastSavedUniversalTime);

            // Enregistrez le classeur
            workbook.Save("LastSavedUniversalTimeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


