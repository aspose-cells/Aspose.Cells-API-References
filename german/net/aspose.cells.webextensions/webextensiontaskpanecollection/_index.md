---
title: "Klasse WebExtensionTaskPaneCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.WebExtensions.WebExtensionTaskPaneCollection Klasse. Stellt die Liste der Task-Panes dar"
type: docs
url: /de/net/aspose.cells.webextensions/webextensiontaskpanecollection/
---
## WebExtensionTaskPaneCollection class

Stellt die Liste der Taskpanes dar.

```csharp
public class WebExtensionTaskPaneCollection : CollectionBase<WebExtensionTaskPane>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensiontaskpanecollection/item/) { get; } | Liefert das Task-Pane anhand des angegebenen Index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensiontaskpanecollection/add/)() | Fügt ein Task-Pane hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionTaskPane) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(WebExtensionTaskPane, IComparer&lt;WebExtensionTaskPane&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, WebExtensionTaskPane, IComparer&lt;WebExtensionTaskPane&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(WebExtensionTaskPane) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionTaskPane[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(WebExtensionTaskPane[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, WebExtensionTaskPane[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;WebExtensionTaskPane&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;WebExtensionTaskPane&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;WebExtensionTaskPane&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;WebExtensionTaskPane&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;WebExtensionTaskPane&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;WebExtensionTaskPane&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;WebExtensionTaskPane&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;WebExtensionTaskPane&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;WebExtensionTaskPane&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;WebExtensionTaskPane&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionTaskPane) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionTaskPane, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(WebExtensionTaskPane, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionTaskPane) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionTaskPane, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(WebExtensionTaskPane, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.WebExtensions;

namespace AsposeCellsExamples
{
    public class WebExtensionsClassWebExtensionTaskPaneCollectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge einige Web-Extension-Task-Panes hinzu
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            
            // Füge drei Task-Panes hinzu (Demo-Zwecke)
            taskPanes.Add();
            taskPanes.Add();
            taskPanes.Add();

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
            
            Console.WriteLine("WebExtensionTaskPaneCollection demo executed successfully.");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtensionTaskPane](../webextensiontaskpane/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


