---
title: "Klasse TextBoxCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.TextBoxCollection-Klasse. Kapselt eine Sammlung von TextBox-Objekten"
type: docs
url: /de/net/aspose.cells.drawing/textboxcollection/
---
## TextBoxCollection class

Kapselt eine Sammlung von [`TextBox`](../textbox/) Objekten.

```csharp
public class TextBoxCollection : CollectionBase<TextBox>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/textboxcollection/item/) { get; } | Liest das [`TextBox`](../textbox/) Element am angegebenen Index. (2 Indexer) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.cells.drawing/textboxcollection/add/)(int, int, int, int) | Fügt der Sammlung ein TextBox hinzu. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TextBox) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TextBox, IComparer&lt;TextBox&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TextBox, IComparer&lt;TextBox&gt;) |  |
| [Clear](../../aspose.cells.drawing/textboxcollection/clear/#clear)() | Löscht alle TextBoxen. (2 Methoden) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(TextBox) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TextBox[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TextBox[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, TextBox[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;TextBox&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;TextBox&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;TextBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;TextBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;TextBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;TextBox&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;TextBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;TextBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;TextBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;TextBox&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TextBox) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TextBox, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TextBox, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TextBox) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TextBox, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TextBox, int, int) |  |
| [RemoveAt](../../aspose.cells.drawing/textboxcollection/removeat/#removeat)(int) | Entfernt ein TextBox aus der Datei. (2 Methoden) |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class TextBoxCollectionDemo
    {
        public static void TextBoxCollectionExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            
            // Hole das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Liest das TextBoxCollection-Objekt
            TextBoxCollection textBoxCollection = worksheet.TextBoxes;
            
            // Fügt ein TextBox zur Sammlung hinzu
            int textBoxIndex = textBoxCollection.Add(1, 1, 50, 100);
            
            // Greift auf das hinzugefügte TextBox zu
            TextBox textBox = textBoxCollection[textBoxIndex];
            
            // Setzen Sie einige Eigenschaften der TextBox
            textBox.Text = "Hello, Aspose!";
            textBox.Font.Name = "Arial";
            textBox.Font.Size = 12;
            textBox.Font.IsBold = true;
            
            // Durchlaufen Sie alle TextBoxen in der Sammlung
            foreach (TextBox tbox in textBoxCollection)
            {
                // Führen Sie Vorgänge für jede TextBox aus
                Console.WriteLine(tbox.Text);
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("TextBoxCollectionExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TextBox](../textbox/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


