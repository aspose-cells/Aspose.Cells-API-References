---
title: "Klasse HtmlTableLoadOptionCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HtmlTableLoadOptionCollection Klasse. Stellt die Tabellenoptionen beim Importieren von HTML dar"
type: docs
url: /de/net/aspose.cells/htmltableloadoptioncollection/
---
## HtmlTableLoadOptionCollection class

Stellt die Tabellenoptionen beim Importieren von HTML dar.

```csharp
public class HtmlTableLoadOptionCollection : CollectionBase<HtmlTableLoadOption>
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [HtmlTableLoadOptionCollection](htmltableloadoptioncollection/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/htmltableloadoptioncollection/item/) { get; } | Liest das [`HtmlTableLoadOption`](../htmltableloadoption/) Element am angegebenen Index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [TableToListObject](../../aspose.cells/htmltableloadoptioncollection/tabletolistobject/) { get; set; } | Gibt an, ob Listenobjekte aus importierten Tabellen generiert werden sollen. Der Standardwert ist false. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add)(HtmlTableLoadOption) | (**Obsolete.**) Fügt ein HtmlTableLoadOption zu dieser Sammlung hinzu. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_1)(int) | Füge ein HtmlTableLoadOption zur Liste hinzu. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_4)(string) | Füge ein HtmlTableLoadOption zur Liste hinzu. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_2)(int, int) | Füge ein HtmlTableLoadOption zur Liste hinzu. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_5)(string, int) | Füge ein HtmlTableLoadOption zur Liste hinzu. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_3)(int, int, int) | Füge ein HtmlTableLoadOption zur Liste hinzu. |
| [Add](../../aspose.cells/htmltableloadoptioncollection/add/#add_6)(string, int, int) | Füge ein HtmlTableLoadOption zur Liste hinzu. |
| [AddTableLoadOption](../../aspose.cells/htmltableloadoptioncollection/addtableloadoption/)(HtmlTableLoadOption) | Fügt ein HtmlTableLoadOption zu dieser Sammlung hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, HtmlTableLoadOption, IComparer&lt;HtmlTableLoadOption&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(HtmlTableLoadOption) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(HtmlTableLoadOption[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, HtmlTableLoadOption[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;HtmlTableLoadOption&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(HtmlTableLoadOption, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(HtmlTableLoadOption, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlTableLoadOptionCollectionDemo
    {
        public static void HtmlTableLoadOptionCollectionExample()
        {
            // Erstelle ein neues Workbook
            Workbook workbook = new Workbook();

            // Erstelle HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Greife auf die HtmlTableLoadOptionCollection-Instanz zu
            HtmlTableLoadOptionCollection tableLoadOptions = loadOptions.TableLoadOptions;

            // Setze die TableToListObject-Eigenschaft
            tableLoadOptions.TableToListObject = true;

            // Füge eine neue HtmlTableLoadOption per Tabellenindex hinzu
            int index1 = tableLoadOptions.Add(0);

            // Füge eine neue HtmlTableLoadOption per Tabellen-ID hinzu
            int index2 = tableLoadOptions.Add("tableId");

            // Füge eine neue HtmlTableLoadOption per Tabellenindex und Zielblattindex hinzu
            int index3 = tableLoadOptions.Add(1, 1);

            // Füge eine neue HtmlTableLoadOption per Tabellen-ID und Zielblattindex hinzu
            int index4 = tableLoadOptions.Add("tableId2", 2);

            // Füge eine neue HtmlTableLoadOption per Tabellenindex, Zielblattindex und Ursprungsblattindex hinzu
            int index5 = tableLoadOptions.Add(2, 2, 0);

            // Füge eine neue HtmlTableLoadOption per Tabellen-ID, Zielblattindex und Ursprungsblattindex hinzu
            int index6 = tableLoadOptions.Add("tableId3", 3, 1);

            // Greife auf die HtmlTableLoadOption an einem bestimmten Index zu
            HtmlTableLoadOption option = tableLoadOptions[index1];

            // Setze Eigenschaften der HtmlTableLoadOption
            option.TableIndex = 0;
            option.Id = "tableId";
            option.Name = "TableName";
            option.OriginalSheetIndex = 0;
            option.TargetSheetIndex = 1;
            option.TableToListObject = true;

            // Laden Sie eine HTML-Datei in die Arbeitsmappe mit den Ladeoptionen
            workbook = new Workbook("HtmlTableLoadOptionCollectionExample_original.html", loadOptions);

            // Speichere die Arbeitsmappe
            workbook.Save("HtmlTableLoadOptionCollectionExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [HtmlTableLoadOption](../htmltableloadoption/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


