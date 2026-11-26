---
title: "Clase TextBoxCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.TextBoxCollection. Encapsula una colección de objetos TextBox"
type: docs
url: /es/net/aspose.cells.drawing/textboxcollection/
---
## TextBoxCollection class

Encapsula una colección de objetos [`TextBox`](../textbox/).

```csharp
public class TextBoxCollection : CollectionBase<TextBox>
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/textboxcollection/item/) { get; } | Obtiene el elemento [`TextBox`](../textbox/) en el índice especificado. (2 indexadores) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.drawing/textboxcollection/add/)(int, int, int, int) | Agrega un cuadro de texto a la colección. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TextBox) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TextBox, IComparer&lt;TextBox&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TextBox, IComparer&lt;TextBox&gt;) |  |
| [Clear](../../aspose.cells.drawing/textboxcollection/clear/#clear)() | Borra todos los cuadros de texto. (2 métodos) |
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
| [RemoveAt](../../aspose.cells.drawing/textboxcollection/removeat/#removeat)(int) | Elimina un cuadro de texto del archivo. (2 métodos) |

### Ejemplos

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
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            
            // Obtener la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtén el objeto TextBoxCollection
            TextBoxCollection textBoxCollection = worksheet.TextBoxes;
            
            // Agrega un TextBox a la colección
            int textBoxIndex = textBoxCollection.Add(1, 1, 50, 100);
            
            // Accede al TextBox agregado
            TextBox textBox = textBoxCollection[textBoxIndex];
            
            // Establece algunas propiedades del TextBox
            textBox.Text = "Hello, Aspose!";
            textBox.Font.Name = "Arial";
            textBox.Font.Size = 12;
            textBox.Font.IsBold = true;
            
            // Itera a través de todos los TextBoxes en la colección
            foreach (TextBox tbox in textBoxCollection)
            {
                // Realiza operaciones en cada TextBox
                Console.WriteLine(tbox.Text);
            }
            
            // Guarda el libro de trabajo
            workbook.Save("TextBoxCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TextBox](../textbox/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


