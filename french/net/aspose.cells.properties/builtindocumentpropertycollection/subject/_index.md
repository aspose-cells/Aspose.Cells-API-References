---
title: "BuiltInDocumentPropertyCollection.Subject"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "BuiltInDocumentPropertyCollection property. Obtient ou définit le sujet du document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/subject/
---
## BuiltInDocumentPropertyCollection.Subject property

Obtient ou définit le sujet du document.

```csharp
public string Subject { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertySubjectDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Définir les propriétés de document intégrées
            workbook.BuiltInDocumentProperties.Subject = "LiteraTest";
            workbook.BuiltInDocumentProperties.Title = "LiteraTest";

            // Enregistrez le classeur
            string outputPath = "output.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            // Chargez le classeur enregistré pour vérifier les propriétés
            using (Workbook loadedWorkbook = new Workbook(outputPath))
            {
                string subject = loadedWorkbook.BuiltInDocumentProperties.Subject;
                string title = loadedWorkbook.BuiltInDocumentProperties.Title;

                Console.WriteLine("Subject: " + subject);
                Console.WriteLine("Title: " + title);
            }
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


