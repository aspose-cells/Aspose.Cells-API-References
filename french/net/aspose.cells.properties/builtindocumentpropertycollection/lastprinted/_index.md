---
title: "BuiltInDocumentPropertyCollection.LastPrinted"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Obtient ou définit la date à laquelle le document a été imprimé pour la dernière fois dans le fuseau horaire local"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/lastprinted/
---
## BuiltInDocumentPropertyCollection.LastPrinted property

Obtient ou définit la date à laquelle le document a été imprimé pour la dernière fois dans le fuseau horaire local.

```csharp
public DateTime LastPrinted { get; set; }
```

### Remarques

Si le document n’a jamais été imprimé, cette propriété renverra DateTime.MinValue.

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastPrintedDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Définir les propriétés de document intégrées
            workbook.BuiltInDocumentProperties.CreatedTime = DateTime.Now;
            workbook.BuiltInDocumentProperties.LastPrinted = DateTime.Now.AddDays(-1); // Set to yesterday
            workbook.BuiltInDocumentProperties.LastSavedTime = DateTime.Now;

            // Afficher la propriété LastPrinted
            Console.WriteLine("Last printed: " + workbook.BuiltInDocumentProperties.LastPrinted);

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


