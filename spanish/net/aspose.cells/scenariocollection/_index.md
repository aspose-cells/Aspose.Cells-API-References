---
title: "Clase ScenarioCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.ScenarioCollection. Representa la lista de escenarios"
type: docs
url: /es/net/aspose.cells/scenariocollection/
---
## ScenarioCollection class

Representa la lista de escenarios.

```csharp
public class ScenarioCollection : CollectionBase<Scenario>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [ActiveIndex](../../aspose.cells/scenariocollection/activeindex/) { get; set; } | Obtiene y establece cuál escenario está seleccionado. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/scenariocollection/item/) { get; } | Obtiene el objeto [`Scenario`](../scenario/) por el índice. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [LastSelected](../../aspose.cells/scenariocollection/lastselected/) { get; set; } | Indica cuál escenario fue seleccionado por última vez por el usuario para ejecutarse/mostrarse. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells/scenariocollection/add/)(string) | Agrega un escenario. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Scenario) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Scenario, IComparer&lt;Scenario&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Scenario, IComparer&lt;Scenario&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Scenario) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Scenario[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Scenario[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Scenario[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Scenario&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Scenario&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Scenario&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Scenario&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Scenario&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Scenario&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Scenario&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Scenario&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Scenario&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Scenario&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Scenario) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Scenario, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Scenario, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Scenario) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Scenario, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Scenario, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioCollectionDemo
    {
        public static void ScenarioCollectionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Accede a la ScenarioCollection de la hoja de cálculo
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Agrega un nuevo escenario a la colección
            int scenarioIndex = scenarios.Add("Scenario1");

            // Accede al escenario recién agregado
            Scenario scenario = scenarios[scenarioIndex];

            // Establece algunas propiedades para el escenario
            scenario.Comment = "This is a test scenario.";
            scenario.IsHidden = false;

            // Establece el índice del escenario activo
            scenarios.ActiveIndex = scenarioIndex;

            // Establece el índice del último escenario seleccionado
            scenarios.LastSelected = scenarioIndex;

            // Guarda el libro de trabajo
            workbook.Save("ScenarioCollectionExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Scenario](../scenario/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


