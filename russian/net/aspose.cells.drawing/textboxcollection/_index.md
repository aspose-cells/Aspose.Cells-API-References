---
title: "Класс TextBoxCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Drawing.TextBoxCollection. Инкапсулирует коллекцию объектов TextBox."
type: docs
url: /ru/net/aspose.cells.drawing/textboxcollection/
---
## TextBoxCollection class

Инкапсулирует коллекцию объектов [`TextBox`](../textbox/).

```csharp
public class TextBoxCollection : CollectionBase<TextBox>
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/textboxcollection/item/) { get; } | Получает элемент [`TextBox`](../textbox/) по указанному индексу. (2 индексатора) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.drawing/textboxcollection/add/)(int, int, int, int) | Добавляет текстовое поле в коллекцию. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TextBox) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TextBox, IComparer&lt;TextBox&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TextBox, IComparer&lt;TextBox&gt;) |  |
| [Clear](../../aspose.cells.drawing/textboxcollection/clear/#clear)() | Очищает все текстовые поля. (2 метода) |
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
| [RemoveAt](../../aspose.cells.drawing/textboxcollection/removeat/#removeat)(int) | Удаляет текстовое поле из файла. (2 метода) |

### Примеры

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
            // Создание объекта Workbook
            Workbook workbook = new Workbook();
            
            // Получить первый лист
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Получить объект TextBoxCollection
            TextBoxCollection textBoxCollection = worksheet.TextBoxes;
            
            // Добавить TextBox в коллекцию
            int textBoxIndex = textBoxCollection.Add(1, 1, 50, 100);
            
            // Получить доступ к добавленному TextBox
            TextBox textBox = textBoxCollection[textBoxIndex];
            
            // Установить некоторые свойства TextBox
            textBox.Text = "Hello, Aspose!";
            textBox.Font.Name = "Arial";
            textBox.Font.Size = 12;
            textBox.Font.IsBold = true;
            
            // Итерировать все TextBox в коллекции
            foreach (TextBox tbox in textBoxCollection)
            {
                // Выполнять операции над каждым TextBox
                Console.WriteLine(tbox.Text);
            }
            
            // Сохраните книгу
            workbook.Save("TextBoxCollectionExample.xlsx");
        }
    }
}
```

### См. также

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TextBox](../textbox/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


