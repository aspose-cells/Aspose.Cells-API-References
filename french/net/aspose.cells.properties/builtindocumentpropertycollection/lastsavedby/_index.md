---
title: "BuiltInDocumentPropertyCollection.LastSavedBy"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Obtient ou définit le nom du dernier auteur"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/lastsavedby/
---
## BuiltInDocumentPropertyCollection.LastSavedBy property

Obtient ou définit le nom du dernier auteur.

```csharp
public string LastSavedBy { get; set; }
```

### Remarques

Aspose.Cells ne met pas à jour cette propriété lorsque vous modifiez le document.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastSavedByDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir les propriétés intégrées du document, y compris LastSavedBy
            workbook.BuiltInDocumentProperties.Author = "John Doe";
            workbook.BuiltInDocumentProperties.Title = "Sample Document";
            workbook.BuiltInDocumentProperties.LastSavedBy = "Jane Smith";
            
            // Enregistrez le classeur
            workbook.Save("DocumentPropertiesDemo.xlsx", SaveFormat.Xlsx);
            
            // Chargez le classeur enregistré pour vérifier les propriétés
            Workbook loadedWorkbook = new Workbook("DocumentPropertiesDemo.xlsx");
            
            // Afficher la propriété LastSavedBy
            Console.WriteLine("Last saved by: " + loadedWorkbook.BuiltInDocumentProperties.LastSavedBy);
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


