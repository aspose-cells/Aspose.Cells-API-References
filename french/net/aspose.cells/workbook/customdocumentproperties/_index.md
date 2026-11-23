---
title: "Workbook.CustomDocumentProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Renvoie une collection DocumentProperty qui représente toutes les propriétés de document personnalisées de la feuille de calcul"
type: docs
url: /fr/net/aspose.cells/workbook/customdocumentproperties/
---
## Workbook.CustomDocumentProperties property

Retourne une collection [`DocumentProperty`](../../../aspose.cells.properties/documentproperty/) qui représente toutes les propriétés de document personnalisées de la feuille de calcul.

```csharp
public CustomDocumentPropertyCollection CustomDocumentProperties { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyCustomDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter des propriétés de document personnalisées
            workbook.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.CustomDocumentProperties.Add("Created Date", DateTime.Now);
            workbook.CustomDocumentProperties.Add("Revision", 1);
            workbook.CustomDocumentProperties.Add("Approved", true);
            
            // Accéder et afficher les propriétés personnalisées
            Console.WriteLine("Custom Document Properties:");
            foreach (Aspose.Cells.Properties.DocumentProperty prop in workbook.CustomDocumentProperties)
            {
                Console.WriteLine($"{prop.Name}: {prop.Value} ({prop.Type})");
            }
            
            // Enregistrez le classeur
            workbook.Save("CustomDocumentPropertiesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CustomDocumentPropertyCollection](../../../aspose.cells.properties/customdocumentpropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


