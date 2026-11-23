---
title: "ContentTypePropertyCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "ContentTypePropertyCollection propriété. Obtient la propriété de type de contenu par l'index spécifique"
type: docs
url: /fr/net/aspose.cells.properties/contenttypepropertycollection/item/
---
## ContentTypePropertyCollection indexer (1 of 2)

Obtient la propriété de type de contenu par l'index spécifique.

```csharp
public ContentTypeProperty this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Valeur de retour

La propriété de type de contenu

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Ajouter des propriétés de type de contenu et démontrer l'utilisation de la propriété Item
            int index1 = workbook.ContentTypeProperties.Add("Property1", "Sample Value");
            workbook.ContentTypeProperties[index1].IsNillable = true;
            
            int index2 = workbook.ContentTypeProperties.Add("Property2", 
                DateTime.Now.ToString("yyyy-MM-ddTHH:mm:ss"), "DateTime");
            workbook.ContentTypeProperties[index2].IsNillable = false;
            
            // Accéder aux propriétés en utilisant l'indexeur Item
            Console.WriteLine($"Property1 IsNillable: {workbook.ContentTypeProperties[0].IsNillable}");
            Console.WriteLine($"Property2 IsNillable: {workbook.ContentTypeProperties[1].IsNillable}");
            
            workbook.Save("ContentTypePropertiesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## ContentTypePropertyCollection indexer (2 of 2)

Obtient la propriété de type de contenu par le nom de la propriété.

```csharp
public ContentTypeProperty this[string name] { get; }
```

| Paramètre | Description |
| --- | --- |
| name | Le nom de la propriété. |

### Valeur de retour

La propriété de type de contenu

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class ContentTypePropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Ajouter une propriété de type de contenu
            workbook.ContentTypeProperties.Add("Admin", "Aspose", "text");
            
            // Accéder à la propriété en utilisant l'indexeur Item
            ContentTypeProperty property = workbook.ContentTypeProperties["Admin"];
            
            // Modifier les valeurs de la propriété
            property.Value = "UpdatedValue";
            property.IsNillable = false;
            
            // Enregistrer le classeur
            workbook.Save("ContentTypePropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ContentTypeProperty](../../contenttypeproperty/)
* class [ContentTypePropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


