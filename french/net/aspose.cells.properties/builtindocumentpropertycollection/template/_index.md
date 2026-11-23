---
title: "BuiltInDocumentPropertyCollection.Template"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "BuiltInDocumentPropertyCollection property. Obtient ou définit le nom informatif du modèle de document"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/template/
---
## BuiltInDocumentPropertyCollection.Template property

Obtient ou définit le nom informatif du modèle de document.

```csharp
public string Template { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyTemplateDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux propriétés de document intégrées
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Définir la propriété Template
            builtInProperties.Template = "Standard Template";

            // Définir d'autres propriétés de base pour la démonstration
            builtInProperties.Author = "John Doe";
            builtInProperties.Title = "Template Property Demo";

            // Enregistrez le classeur
            workbook.Save("TemplatePropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


