---
title: "Classe CustomXmlPartCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Markup.CustomXmlPartCollection. Représente une partie de stockage de données XML personnalisée (Custom XML Data Storage Part) dans un package"
type: docs
url: /fr/net/aspose.cells.markup/customxmlpartcollection/
---
## CustomXmlPartCollection class

Représente une partie de stockage de données XML personnalisées (données XML personnalisées dans un package).

```csharp
public class CustomXmlPartCollection : CollectionBase<CustomXmlPart>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.markup/customxmlpartcollection/item/) { get; } | Obtient un élément à l'index spécifié. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.markup/customxmlpartcollection/add/)(byte[], byte[]) | Ajoute un élément à la collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomXmlPart) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomXmlPart, IComparer&lt;CustomXmlPart&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CustomXmlPart, IComparer&lt;CustomXmlPart&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CustomXmlPart) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomXmlPart[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomXmlPart[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CustomXmlPart[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CustomXmlPart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CustomXmlPart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CustomXmlPart&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomXmlPart) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomXmlPart, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomXmlPart, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomXmlPart) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomXmlPart, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomXmlPart, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
| [SelectByID](../../aspose.cells.markup/customxmlpartcollection/selectbyid/)(string) | Obtient un élément par identifiant. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassCustomXmlPartCollectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Obtenez la CustomXmlPartCollection du classeur
            CustomXmlPartCollection customXmlParts = workbook.CustomXmlParts;

            // Créez des données XML d'exemple et un schéma
            byte[] xmlData = System.Text.Encoding.UTF8.GetBytes("<root><item>Test</item></root>");
            byte[] schemaData = System.Text.Encoding.UTF8.GetBytes("<xsd:schema xmlns:xsd='http://www.w3.org/2001/XMLSchema'></xsd:schema>");

            // Ajoutez une nouvelle partie XML personnalisée
            int index = customXmlParts.Add(xmlData, schemaData);

            // Obtenez la partie XML ajoutée par indice
            CustomXmlPart part = customXmlParts[index];

            // Sélectionnez la partie XML par ID (si connu)
            string partId = part.ID;
            CustomXmlPart selectedPart = customXmlParts.SelectByID(partId);

            // Ajoutez une autre partie XML
            byte[] xmlData2 = System.Text.Encoding.UTF8.GetBytes("<data><value>123</value></data>");
            customXmlParts.Add(xmlData2, null);

            // Affichez le nombre de parties XML personnalisées
            Console.WriteLine("Custom XML parts count: " + customXmlParts.Count);

            // Enregistrez le classeur
            workbook.Save("CustomXmlPartCollectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [CustomXmlPart](../customxmlpart/)
* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


