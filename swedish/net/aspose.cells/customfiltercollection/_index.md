---
title: "Klass CustomFilterCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.CustomFilterCollection-klass. Representerar de anpassade filtren"
type: docs
url: /sv/net/aspose.cells/customfiltercollection/
---
## CustomFilterCollection class

Representerar de anpassade filtren.

```csharp
public class CustomFilterCollection : CollectionBase<CustomFilter>
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [CustomFilterCollection](customfiltercollection/)() | (**Föråldrad.**) Skapar en ny instans. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [And](../../aspose.cells/customfiltercollection/and/) { get; set; } | Indikerar om de två kriterierna har ett \"och\"‑förhållande. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/customfiltercollection/item/) { get; } | Hämtar det anpassade filtret på det specifika indexet. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomFilter) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomFilter, IComparer&lt;CustomFilter&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CustomFilter, IComparer&lt;CustomFilter&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CustomFilter) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomFilter[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomFilter[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CustomFilter[], int, int) |  |
| [Custom](../../aspose.cells/customfiltercollection/custom/)(FilterOperatorType, object, bool, FilterOperatorType, object) | Filtrerar en lista med anpassade kriterier. |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CustomFilter&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CustomFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CustomFilter&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CustomFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CustomFilter&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomFilter) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomFilter, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomFilter, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomFilter) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomFilter, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomFilter, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassCustomFilterCollectionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Numbers");
            sheet.Cells["A2"].PutValue(10);
            sheet.Cells["A3"].PutValue(20);
            sheet.Cells["A4"].PutValue(30);
            sheet.Cells["A5"].PutValue(40);
            sheet.Cells["A6"].PutValue(50);

            // Aktivera autofilter först
            sheet.AutoFilter.Range = "A1:A6";
            
            // Skapa anpassade filter
            sheet.AutoFilter.Custom(0, FilterOperatorType.GreaterOrEqual, "30");
            sheet.AutoFilter.Custom(0, FilterOperatorType.LessOrEqual, "40");

            // Hämta filter via reflektion eftersom direkt metod inte är tillgänglig
            var filterField = sheet.AutoFilter.GetType().GetField("m_customFilters", 
                System.Reflection.BindingFlags.NonPublic | System.Reflection.BindingFlags.Instance);
            var filters = (CustomFilterCollection)filterField.GetValue(sheet.AutoFilter);

            // Tillämpa filter
            Cells_Type_CustomFilterCollection(sheet, filters);

            // Spara arbetsboken
            workbook.Save("CustomFilterDemo.xlsx");
        }

        private static void Cells_Type_CustomFilterCollection(Worksheet sheet, CustomFilterCollection filters)
        {
            Console.WriteLine("Applying custom filters:");
            if (filters != null)
            {
                for (int i = 0; i < filters.Count; i++)
                {
                    Console.WriteLine($"Filter: {filters[i].FilterOperatorType}, Criteria: {filters[i].Criteria}");
                }
            }
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [CustomFilter](../customfilter/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


