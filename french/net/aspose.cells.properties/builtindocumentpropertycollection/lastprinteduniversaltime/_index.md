---
title: "BuiltInDocumentPropertyCollection.LastPrintedUniversalTime"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété BuiltInDocumentPropertyCollection. Obtient ou définit l'heure universelle à laquelle le document a été imprimé pour la dernière fois"
type: docs
url: /fr/net/aspose.cells.properties/builtindocumentpropertycollection/lastprinteduniversaltime/
---
## BuiltInDocumentPropertyCollection.LastPrintedUniversalTime property

Obtient ou définit l'heure universelle à laquelle le document a été imprimé pour la dernière fois.

```csharp
public DateTime LastPrintedUniversalTime { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class BuiltInDocumentPropertyCollectionPropertyLastPrintedUniversalTimeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Accéder aux propriétés de document intégrées
            BuiltInDocumentPropertyCollection builtInProperties = workbook.BuiltInDocumentProperties;

            // Définir la propriété LastPrintedUniversalTime
            DateTime currentUtcTime = DateTime.UtcNow;
            builtInProperties.LastPrintedUniversalTime = currentUtcTime;

            // Afficher la valeur définie
            Console.WriteLine("LastPrintedUniversalTime set to: " + builtInProperties.LastPrintedUniversalTime);

            // Enregistrez le classeur
            workbook.Save("LastPrintedUniversalTimeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [BuiltInDocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


