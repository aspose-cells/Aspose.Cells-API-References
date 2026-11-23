---
title: "DocumentPropertyCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DocumentPropertyCollection. Retourne un objet DocumentProperty par le nom de la propriété"
type: docs
url: /fr/net/aspose.cells.properties/documentpropertycollection/item/
---
## DocumentPropertyCollection indexer (1 of 2)

Retourne un objet [`DocumentProperty`](../../documentproperty/) par le nom de la propriété.

```csharp
public virtual DocumentProperty this[string name] { get; }
```

| Paramètre | Description |
| --- | --- |
| name | Le nom de la propriété à récupérer, insensible à la casse. |

### Remarques

Retourne null si aucune propriété avec le nom spécifié n'est trouvée.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            string key = "TemplateGUID";
            object value = "TestValue123";

            if (wb.Worksheets.CustomDocumentProperties.Contains(key))
            {
                wb.Worksheets.CustomDocumentProperties[key].Value = value;
            }
            else
            {
                wb.Worksheets.CustomDocumentProperties.Add(key, value.ToString());
            }

            // Vérifier que la valeur a été définie en utilisant la propriété Item
            Console.WriteLine("Property Value: " + wb.Worksheets.CustomDocumentProperties[key].Value);
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)

---

## DocumentPropertyCollection indexer (2 of 2)

Renvoie un objet [`DocumentProperty`](../../documentproperty/) par indice.

```csharp
public DocumentProperty this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| index | Indice basé sur zéro du [`DocumentProperty`](../../documentproperty/) à récupérer. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Properties;

namespace AsposeCellsExamples
{
    public class DocumentPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenir les propriétés de document intégrées
            BuiltInDocumentPropertyCollection properties = workbook.BuiltInDocumentProperties;

            // Définir les propriétés intégrées (pas Ajouter)
            properties.Author = "John Doe";
            properties.Company = "Aspose";
            properties["Version"].Value = "1.0";

            // Accéder aux propriétés en utilisant l'indexeur Item
            Console.WriteLine("Property 0: " + properties[0].Name + " = " + properties[0].Value);
            Console.WriteLine("Property 1: " + properties[1].Name + " = " + properties[1].Value);
            Console.WriteLine("Property 2: " + properties[2].Name + " = " + properties[2].Value);

            // Accède à la propriété par son nom
            DocumentProperty authorProp = properties["Author"];
            Console.WriteLine("Author property: " + authorProp.Value);

            // Modifier une propriété
            properties["Version"].Value = "2.0";
            Console.WriteLine("Updated Version: " + properties["Version"].Value);
        }
    }
}
```

### Voir aussi

* class [DocumentProperty](../../documentproperty/)
* class [DocumentPropertyCollection](../)
* namespace [Aspose.Cells.Properties](../../../aspose.cells.properties/)
* assembly [Aspose.Cells](../../../)


