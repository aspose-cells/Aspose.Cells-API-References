---
title: "WebExtensionPropertyCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété WebExtensionPropertyCollection. Obtient la propriété d'extension web par l'index"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensionpropertycollection/item/
---
## WebExtensionPropertyCollection indexer (1 of 2)

Obtient la propriété d'extension web par l'index.

```csharp
public WebExtensionProperty this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'indice. |

### Valeur de retour

La propriété d'extension web.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une collection de propriétés d'extension web
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Ajouter quelques propriétés
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Accéder aux propriétés en utilisant l'indexeur Item
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Modifier les valeurs des propriétés via la collection
            properties[index1].Value = "UpdatedValue1";
            properties[index2].Value = "UpdatedValue2";

            // Démontrer les changements
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property at index 0: Name={0}, Value={1}", 
                properties[index1].Name, properties[index1].Value);
            Console.WriteLine("Property at index 1: Name={0}, Value={1}", 
                properties[index2].Name, properties[index2].Value);

            // Enregistrer le classeur (bien que les propriétés de l'extension web ne soient pas visibles dans le fichier enregistré sans configuration appropriée)
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)

---

## WebExtensionPropertyCollection indexer (2 of 2)

Obtient la propriété de l'extension web.

```csharp
public WebExtensionProperty this[string name] { get; }
```

| Paramètre | Description |
| --- | --- |
| name | Le nom de la propriété. |

### Valeur de retour

La propriété d'extension web.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.WebExtensions;
    using System;

    public class WebExtensionPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une collection de propriétés d'extension web
            WebExtensionPropertyCollection properties = new WebExtensionPropertyCollection();

            // Ajoute des propriétés à la collection
            properties.Add("Property1", "Value1");
            properties.Add("Property2", "Value2");

            // Accéder aux propriétés en utilisant l'indexeur Item
            WebExtensionProperty property1 = properties["Property1"];
            Console.WriteLine("Property1 value: " + property1.Value);

            WebExtensionProperty property2 = properties["Property2"];
            Console.WriteLine("Property2 value: " + property2.Value);

            // Modifier les valeurs des propriétés (note : Item est en lecture seule, nous devons donc utiliser Ajouter/Supprimer)
            properties.RemoveAt("Property1");
            properties.Add("Property1", "NewValue1");

            // Afficher la valeur mise à jour
            property1 = properties["Property1"];
            Console.WriteLine("Updated Property1 value: " + property1.Value);

            // Enregistrez le classeur
            workbook.Save("WebExtensionPropertiesDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [WebExtensionProperty](../../webextensionproperty/)
* class [WebExtensionPropertyCollection](../)
* namespace [Aspose.Cells.WebExtensions](../../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../../)


