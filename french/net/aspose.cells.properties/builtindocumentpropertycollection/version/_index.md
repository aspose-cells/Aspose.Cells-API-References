---
title: "BuiltInDocumentPropertyCollection.Version"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Représente le numéro de version de l'application qui a créé le document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/version/
---
## BuiltInDocumentPropertyCollection.Version property

Représente le numéro de version de l'application qui a créé le document.

```csharp
public string Version { get; set; }
```

### Remarques

Son format est "00.0000", par exemple : 12.0000

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyVersionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Définir certaines propriétés du document
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Accéder et afficher la propriété Version
            string version = workbook.BuiltInDocumentProperties.Version;
            Console.WriteLine("Document Version: " + version);
            
            // Enregistrez le classeur
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


