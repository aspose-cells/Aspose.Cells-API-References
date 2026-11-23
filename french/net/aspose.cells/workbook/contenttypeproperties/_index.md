---
title: "Workbook.ContentTypeProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Workbook. Obtient la liste des objets ContentTypeProperty dans le classeur"
type: docs
url: /fr/net/aspose.cells/workbook/contenttypeproperties/
---
## Workbook.ContentTypeProperties property

Obtient la liste des objets [`ContentTypeProperty`](../../../aspose.cells.properties/contenttypeproperty/) dans le classeur.

```csharp
public ContentTypePropertyCollection ContentTypeProperties { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyContentTypePropertiesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Ajouter une propriété chaîne simple
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            // Ajouter une propriété date‑heure avec spécification de type
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Enregistrez le classeur
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ContentTypePropertyCollection](../../../aspose.cells.properties/contenttypepropertycollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


