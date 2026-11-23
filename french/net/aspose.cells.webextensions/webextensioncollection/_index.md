---
title: "Classe WebExtensionCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.WebExtensions.WebExtensionCollection. Représente la liste des extensions web"
type: docs
url: /fr/net/aspose.cells.webextensions/webextensioncollection/
---
## WebExtensionCollection class

Représente la liste des extensions web.

```csharp
public class WebExtensionCollection : CollectionBase<WebExtension>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensioncollection/item/) { get; } | Obtient l'extension web par l'index spécifique. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensioncollection/add/)() | Ajoute une extension web. |
| [AddWebVideoPlayer](../../aspose.cells.webextensions/webextensioncollection/addwebvideoplayer/)(string, bool, int, int) | Ajoute un lecteur vidéo web dans exel. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtension) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtension, IComparer&lt;WebExtension&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, WebExtension, IComparer&lt;WebExtension&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(WebExtension) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtension[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtension[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, WebExtension[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;WebExtension&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;WebExtension&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;WebExtension&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;WebExtension&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;WebExtension&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;WebExtension&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;WebExtension&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;WebExtension&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;WebExtension&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;WebExtension&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtension) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtension, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtension, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtension) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtension, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtension, int, int) |  |
| [RemoveAt](../../aspose.cells.webextensions/webextensioncollection/removeat/#removeat)(int) | Supprime l'extension web par l'index. (2 méthodes) |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WebExtensionsClassWebExtensionCollectionDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la WebExtensionCollection
            WebExtensionCollection webExtensions = workbook.Worksheets.WebExtensions;
            
            // Ajouter une nouvelle extension web
            int index = webExtensions.Add();
            WebExtension webExt = webExtensions[index];
            
            // Définir les propriétés de l'extension web
            webExt.Reference.Id = "wa104104476";
            webExt.Reference.Version = "1.3.0.0";
            webExt.Reference.StoreName = "en-US";
            webExt.Reference.StoreType = WebExtensionStoreType.OMEX;
            
            // Ajouter des propriétés personnalisées
            webExt.Properties.Add("sku", "peoplebar-giant");
            webExt.Properties.Add("theme", "giant-redwhiteblack");
            webExt.Properties.Add("shape", "muscle-people");
            webExt.Properties.Add("layout-element-title", "NUMBERS ABOUT THE APP");
            
            // Créer une forme pour héberger l'extension web
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddShape(MsoDrawingType.WebExtension, 0, 0, 0, 0, 500, 500);
            WebExtensionShape wShape = (WebExtensionShape)shapes[0];
            wShape.WebExtension = webExt;
            
            // Enregistrez le classeur
            workbook.Save("web_extension_demo.xlsx");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtension](../webextension/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


