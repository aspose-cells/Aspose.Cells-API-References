---
title: "DocumentProperty.Value"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DocumentProperty. Obtient ou définit la valeur de la propriété"
type: docs
url: /fr/net/aspose.cells.properties/documentproperty/value/
---
## DocumentProperty.Value property

Obtient ou définit la valeur de la propriété.

```csharp
public object Value { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyPropertyValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accédez aux propriétés de document intégrées
            var hyperlinkBase = workbook.Worksheets.BuiltInDocumentProperties["HyperlinkBase"];
            hyperlinkBase.Value = "http://www.example.com";

            var title = workbook.Worksheets.BuiltInDocumentProperties["Title"];
            title.Value = "Sample Document Title";

            // Enregistrez le classeur
            workbook.Save("DocumentPropertiesDemo.xlsx");

            // Affichez les valeurs définies
            Console.WriteLine("HyperlinkBase: " + hyperlinkBase.Value);
            Console.WriteLine("Title: " + title.Value);
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


