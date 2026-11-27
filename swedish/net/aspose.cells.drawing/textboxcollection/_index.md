---
title: "Klass TextBoxCollection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.TextBoxCollection klass. Inkapslar en samling av TextBox-objekt"
type: docs
url: /sv/net/aspose.cells.drawing/textboxcollection/
---
## TextBoxCollection class

Inkapslar en samling av [`TextBox`](../textbox/) objekt.

```csharp
public class TextBoxCollection : CollectionBase<TextBox>
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/textboxcollection/item/) { get; } | Hämtar [`TextBox`](../textbox/) elementet vid det angivna indexet. (2 indexerare) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Add](../../aspose.cells.drawing/textboxcollection/add/)(int, int, int, int) | Lägger till en textruta i samlingen. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TextBox) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TextBox, IComparer&lt;TextBox&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TextBox, IComparer&lt;TextBox&gt;) |  |
| [Clear](../../aspose.cells.drawing/textboxcollection/clear/#clear)() | Rensa alla textrutor. (2 metoder) |
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
| [RemoveAt](../../aspose.cells.drawing/textboxcollection/removeat/#removeat)(int) | Ta bort en textruta från filen. (2 metoder) |

### Exempel

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
            // Instansiering av ett Workbook-objekt
            Workbook workbook = new Workbook();
            
            // Hämta det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta TextBoxCollection-objektet
            TextBoxCollection textBoxCollection = worksheet.TextBoxes;
            
            // Lägg till en TextBox i samlingen
            int textBoxIndex = textBoxCollection.Add(1, 1, 50, 100);
            
            // Åtkomst till den tillagda TextBoxen
            TextBox textBox = textBoxCollection[textBoxIndex];
            
            // Ställ in några egenskaper för TextBoxen
            textBox.Text = "Hello, Aspose!";
            textBox.Font.Name = "Arial";
            textBox.Font.Size = 12;
            textBox.Font.IsBold = true;
            
            // Iterera genom alla TextBoxes i samlingen
            foreach (TextBox tbox in textBoxCollection)
            {
                // Utför operationer på varje TextBox
                Console.WriteLine(tbox.Text);
            }
            
            // Spara arbetsboken
            workbook.Save("TextBoxCollectionExample.xlsx");
        }
    }
}
```

### Se även

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TextBox](../textbox/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


