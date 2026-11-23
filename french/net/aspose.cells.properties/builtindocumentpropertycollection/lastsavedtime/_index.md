---
title: "BuiltInDocumentPropertyCollection.LastSavedTime"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Obtient ou définit l'heure de la dernière sauvegarde dans le fuseau horaire local"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/lastsavedtime/
---
## BuiltInDocumentPropertyCollection.LastSavedTime property

Obtient ou définit l'heure de la dernière sauvegarde dans le fuseau horaire local.

```csharp
public DateTime LastSavedTime { get; set; }
```

### Remarques

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedTimeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Définir les propriétés de document intégrées
            workbook.BuiltInDocumentProperties.CreatedTime = new DateTime(2023, 1, 1);
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now;
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;

            // Afficher la propriété LastSavedTime
            Console.WriteLine("Last Saved Time: " + 
                workbook.BuiltInDocumentProperties.LastSavedTime);

            // Enregistrez le classeur
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


