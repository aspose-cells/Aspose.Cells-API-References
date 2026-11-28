---
title: "Sınıf ScenarioCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.ScenarioCollection sınıfı. Senaryoların listesini temsil eder."
type: docs
url: /tr/net/aspose.cells/scenariocollection/
---
## ScenarioCollection class

Senaryoların listesini temsil eder.

```csharp
public class ScenarioCollection : CollectionBase<Scenario>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActiveIndex](../../aspose.cells/scenariocollection/activeindex/) { get; set; } | Seçilen senaryoyu alır ve ayarlar. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/scenariocollection/item/) { get; } | İndeksle [`Scenario`](../scenario/) nesnesini alır. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [LastSelected](../../aspose.cells/scenariocollection/lastselected/) { get; set; } | Kullanıcı tarafından çalıştırılmak/gösterilmek üzere son seçilen senaryoyu belirtir. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells/scenariocollection/add/)(string) | Bir senaryo ekler. |
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

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioCollectionDemo
    {
        public static void ScenarioCollectionExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasının ScenarioCollection'ına erişin
            ScenarioCollection scenarios = worksheet.Scenarios;

            // Koleksiyona yeni bir senaryo ekleyin
            int scenarioIndex = scenarios.Add("Scenario1");

            // Yeni eklenen senaryoya erişin
            Scenario scenario = scenarios[scenarioIndex];

            // Senaryo için bazı özellikleri ayarlayın
            scenario.Comment = "This is a test scenario.";
            scenario.IsHidden = false;

            // Etkin senaryo indeksini ayarlayın
            scenarios.ActiveIndex = scenarioIndex;

            // Son seçilen senaryo indeksini ayarlayın
            scenarios.LastSelected = scenarioIndex;

            // Çalışma kitabını kaydedin
            workbook.Save("ScenarioCollectionExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Scenario](../scenario/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


