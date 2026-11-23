---
title: "SmartTagPropertyCollection.Item"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SmartTagPropertyCollection. Obtient un objet SmartTagProperty"
type: docs
url: /fr/net/aspose.cells.markup/smarttagpropertycollection/item/
---
## SmartTagPropertyCollection indexer (1 of 2)

Obtient un objet [`SmartTagProperty`](../../smarttagproperty/).

```csharp
public SmartTagProperty this[int index] { get; }
```

| Paramètre | Description |
| --- | --- |
| indice | L'index |

### Valeur de retour

Renvoie un objet [`SmartTagProperty`](../../smarttagproperty/).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Créer une collection de propriétés de smart tag
            SmartTagPropertyCollection properties = new SmartTagPropertyCollection();

            // Ajoute des propriétés à la collection
            int index1 = properties.Add("Property1", "Value1");
            int index2 = properties.Add("Property2", "Value2");

            // Accéder aux propriétés en utilisant l'indexeur Item
            SmartTagProperty property1 = properties[index1];
            SmartTagProperty property2 = properties[index2];

            // Afficher les valeurs actuelles des propriétés
            Console.WriteLine("Property1 Name: " + property1.Name);
            Console.WriteLine("Property1 Value: " + property1.Value);
            Console.WriteLine("Property2 Name: " + property2.Name);
            Console.WriteLine("Property2 Value: " + property2.Value);

            // Remarque : La propriété Item est en lecture seule, donc nous ne pouvons pas lui assigner directement
            // À la place, nous pouvons modifier les propriétés des objets SmartTagProperty retournés
            property1.Value = "UpdatedValue1";
            property2.Value = "UpdatedValue2";

            // Afficher les valeurs mises à jour
            Console.WriteLine("\nAfter modification:");
            Console.WriteLine("Property1 Value: " + properties[index1].Value);
            Console.WriteLine("Property2 Value: " + properties[index2].Value);

            // Enregistrer le classeur (bien que les smart tags ne soient pas stockés visiblement lors d'un enregistrement simple)
            workbook.Save("SmartTagPropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagPropertyCollection indexer (2 of 2)

Obtient un objet [`SmartTagProperty`](../../smarttagproperty/) par le nom de la propriété.

```csharp
public SmartTagProperty this[string name] { get; }
```

| Paramètre | Description |
| --- | --- |
| name | Le nom de la propriété. |

### Valeur de retour

Renvoie un objet [`SmartTagProperty`](../../smarttagproperty/).

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagPropertyCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Créer un paramètre de smart tag et ajouter un smart tag
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
                int smartTagIndex = smartTagSetting.Add(0, 0);
                SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
                smartTags.Add("http://example.com", "example");

                // Obtenir le smart tag et ses propriétés
                SmartTag smartTag = smartTags[0];
                SmartTagPropertyCollection properties = smartTag.Properties;

                // Ajouter quelques propriétés pour démontrer la propriété Item
                properties.Add("Author", "John Doe");
                properties.Add("Version", "1.0");

                // Accéder aux propriétés en utilisant l'indexeur Item (par indice)
                SmartTagProperty firstProperty = properties[0];
                SmartTagProperty secondProperty = properties[1];

                // Affiche les valeurs des propriétés
                Console.WriteLine("First Property Name: " + firstProperty.Name);
                Console.WriteLine("First Property Value: " + firstProperty.Value);
                Console.WriteLine("Second Property Name: " + secondProperty.Name);
                Console.WriteLine("Second Property Value: " + secondProperty.Value);

                // Enregistrez le classeur
                workbook.Save("SmartTagItemDemo.xlsx");
                Console.WriteLine("SmartTagItemDemo.xlsx created successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Voir aussi

* class [SmartTagProperty](../../smarttagproperty/)
* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


