---
title: "Klasse NameCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.NameCollection‑Klasse. Stellt eine Sammlung aller Name‑Objekte im Tabellenblatt dar."
type: docs
url: /de/net/aspose.cells/namecollection/
---
## NameCollection class

Stellt eine Sammlung aller [`Name`](../name/)-Objekte im Tabellenblatt dar.

```csharp
public class NameCollection : CollectionBase<Name>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/namecollection/item/) { get; } | Liest das [`Name`](../name/)-Element am angegebenen Index. (2 Indexer) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells/namecollection/add/)(string) | Definiert einen neuen Namen. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Name, IComparer&lt;Name&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Name, IComparer&lt;Name&gt;) |  |
| [Clear](../../aspose.cells/namecollection/clear/#clear)() | Entfernt alle definierten Namen, die von Formeln und Datenquellen nicht referenziert werden. Wenn der definierte Name referenziert wird, setzen wir nur Name.ReferTo auf null und blenden ihn aus. (2 Methoden) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Name) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Name[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Name[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Name&gt;) |  |
| [Filter](../../aspose.cells/namecollection/filter/)(NameScopeType, int) | Ruft alle definierten Namen nach Geltungsbereich ab. |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Name&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Name&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Name&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Name, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Name, int, int) |  |
| [Remove](../../aspose.cells/namecollection/remove/#remove)(string) | Entfernt den Namen. |
| [Remove](../../aspose.cells/namecollection/remove/#remove_1)(string[]) | Entfernt ein Array von Namen. |
| [RemoveAt](../../aspose.cells/namecollection/removeat/#removeat)(int) | Entfernt den Namen am spezifischen Index. (2 Methoden) |
| [RemoveDuplicateNames](../../aspose.cells/namecollection/removeduplicatenames/)() | Entfernt die doppelten definierten Namen |
| [Sort](../../aspose.cells/namecollection/sort/)() | Sortiert definierte Namen. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameCollectionDemo
    {
        public static void NameCollectionExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greift auf die Arbeitsblatt‑Sammlung zu
            WorksheetCollection worksheets = workbook.Worksheets;
            
            // Greift auf die Namenssammlung zu
            NameCollection names = worksheets.Names;
            
            // Fügt einen neuen Namen zur Sammlung hinzu
            int nameIndex = names.Add("MyNamedRange");
            Name name = names[nameIndex];
            
            // Setzt die refers to‑Eigenschaft für den Namen
            name.RefersTo = "=Sheet1!$A$1:$A$10";
            
            // Greift zu und ändert Eigenschaften des Namens
            name.Comment = "This is a named range for demonstration.";
            name.IsVisible = true;
            
            // Fügt einen weiteren Namen hinzu
            int anotherNameIndex = names.Add("AnotherNamedRange");
            Name anotherName = names[anotherNameIndex];
            anotherName.RefersTo = "=Sheet1!$B$1:$B$10";
            
            // Entfernt einen Namen nach Text
            names.Remove("AnotherNamedRange");
            
            // Entfernt einen Namen nach Index
            names.RemoveAt(nameIndex);
            
            // Löscht alle Namen
            names.Clear();
            
            // Speichere die Arbeitsmappe
            workbook.Save("NameCollectionExample.xlsx");

            return;
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Name](../name/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


