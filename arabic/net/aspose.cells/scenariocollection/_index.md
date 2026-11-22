---
title: "الفئة ScenarioCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ScenarioCollection. تمثل قائمة السيناريوهات"
type: docs
url: /ar/net/aspose.cells/scenariocollection/
---
## ScenarioCollection class

يمثل قائمة السيناريوهات.

```csharp
public class ScenarioCollection : CollectionBase<Scenario>
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ActiveIndex](../../aspose.cells/scenariocollection/activeindex/) { get; set; } | يحصل على ويضبط أي سيناريو تم اختياره. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/scenariocollection/item/) { get; } | يحصل على كائن [`Scenario`](../scenario/) حسب الفهرس. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [LastSelected](../../aspose.cells/scenariocollection/lastselected/) { get; set; } | يشير إلى أي سيناريو تم اختياره آخر مرة من قبل المستخدم لتشغيله/عرضه. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells/scenariocollection/add/)(string) | يضيف سيناريو. |
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

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ScenarioCollectionDemo
    {
        public static void ScenarioCollectionExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى ScenarioCollection في ورقة العمل
            ScenarioCollection scenarios = worksheet.Scenarios;

            // أضف سيناريو جديد إلى المجموعة
            int scenarioIndex = scenarios.Add("Scenario1");

            // الوصول إلى السيناريو المضاف حديثًا
            Scenario scenario = scenarios[scenarioIndex];

            // ضبط بعض الخصائص للسيناريو
            scenario.Comment = "This is a test scenario.";
            scenario.IsHidden = false;

            // ضبط فهرس السيناريو النشط
            scenarios.ActiveIndex = scenarioIndex;

            // ضبط فهرس السيناريو المختار آخرًا
            scenarios.LastSelected = scenarioIndex;

            // احفظ المصنف
            workbook.Save("ScenarioCollectionExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Scenario](../scenario/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


