---
title: "Clase WebExtensionTaskPaneCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.WebExtensions.WebExtensionTaskPaneCollection. Representa la lista de paneles de tareas"
type: docs
url: /es/net/aspose.cells.webextensions/webextensiontaskpanecollection/
---
## WebExtensionTaskPaneCollection class

Representa la lista de paneles de tareas.

```csharp
public class WebExtensionTaskPaneCollection : CollectionBase<WebExtensionTaskPane>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.webextensions/webextensiontaskpanecollection/item/) { get; } | Obtiene el panel de tareas por el índice específico. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.webextensions/webextensiontaskpanecollection/add/)() | Agrega un panel de tareas. |
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

### Ejemplos

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
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos paneles de tareas de extensiones web
            WebExtensionTaskPaneCollection taskPanes = workbook.Worksheets.WebExtensionTaskPanes;
            
            // Agregar tres paneles de tareas (con fines de demostración)
            taskPanes.Add();
            taskPanes.Add();
            taskPanes.Add();

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
            
            Console.WriteLine("WebExtensionTaskPaneCollection demo executed successfully.");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [WebExtensionTaskPane](../webextensiontaskpane/)
* namespace [Aspose.Cells.WebExtensions](../../aspose.cells.webextensions/)
* assembly [Aspose.Cells](../../)


