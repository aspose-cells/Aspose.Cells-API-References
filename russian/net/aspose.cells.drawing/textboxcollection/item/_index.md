---
title: "TextBoxCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TextBoxCollection. Получает элемент TextBox по указанному индексу"
type: docs
url: /ru/net/aspose.cells.drawing/textboxcollection/item/
---
## TextBoxCollection indexer (1 of 2)

Получает элемент [`TextBox`](../../textbox/) по указанному индексу.

```csharp
public TextBox this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Индекс элемента, начиная с нуля. |

### Возвращаемое значение

Элемент по указанному индексу.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте несколько текстовых полей в лист
            int textBoxIndex1 = worksheet.TextBoxes.Add(10, 10, 100, 50);
            TextBox textBox1 = worksheet.TextBoxes[textBoxIndex1];
            textBox1.Text = "TextBox 1";
            
            int textBoxIndex2 = worksheet.TextBoxes.Add(10, 70, 100, 50);
            TextBox textBox2 = worksheet.TextBoxes[textBoxIndex2];
            textBox2.Text = "TextBox 2";

            // Получайте доступ к текстовым полям с помощью свойства Item
            TextBoxCollection textBoxCollection = worksheet.TextBoxes;
            int index = textBoxCollection.Count - 1;
            TextBox lastTextBox = textBoxCollection[index];

            // Выведите текст последнего текстового поля
            Console.WriteLine("Last TextBox Text: " + lastTextBox.Text);
        }
    }
}
```

### См. также

* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## TextBoxCollection indexer (2 of 2)

Получает элемент [`TextBox`](../../textbox/) по имени.

```csharp
public TextBox this[string name] { get; }
```

| Параметр | Описание |
| --- | --- |
| name | Имя текстового поля. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextBoxCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте текстовые поля в лист и получите их индексы
            int textBoxIndex1 = worksheet.TextBoxes.Add(10, 10, 100, 50);
            TextBox textBox1 = worksheet.TextBoxes[textBoxIndex1];
            textBox1.Name = "textbox 1";
            textBox1.Text = "First TextBox";

            int textBoxIndex2 = worksheet.TextBoxes.Add(10, 70, 100, 50);
            TextBox textBox2 = worksheet.TextBoxes[textBoxIndex2];
            textBox2.Name = "textbox 2";
            textBox2.Text = "Second TextBox";

            // Получайте доступ к текстовому полю с помощью свойства Item по имени
            string txtboxName = "textbox 1";
            TextBox txb2 = worksheet.TextBoxes[txtboxName];
            if (txb2 != null)
            {
                Console.WriteLine("Found TextBox: " + txb2.Name);
                Console.WriteLine("TextBox Text: " + txb2.Text);
            }
        }
    }
}
```

### См. также

* class [TextBox](../../textbox/)
* class [TextBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


