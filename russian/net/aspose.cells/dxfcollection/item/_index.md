---
title: "DxfCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство DxfCollection. Получает элемент по указанному индексу"
type: docs
url: /ru/net/aspose.cells/dxfcollection/item/
---
## DxfCollection indexer

Получает элемент по указанному индексу.

```csharp
public Style this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс | Указанный индекс. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DxfCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Получить доступ к DxfCollection из рабочей книги
            DxfCollection dxfCollection = workbook.Worksheets.Dxfs;

            // Создать новый стиль (нельзя добавить напрямую в DxfCollection, так как у него нет метода Add)
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            // Стиль автоматически добавляется в коллекцию при создании

            // Получить первый элемент из DxfCollection с помощью свойства Item
            Style firstStyle = dxfCollection[0];
            Console.WriteLine("First style font name: " + firstStyle.Font.Name);

            // Измените стиль через свойство Item (поскольку оно возвращает ссылку)
            firstStyle.Font.Color = System.Drawing.Color.Red;
            firstStyle.Font.IsBold = true;

            // Проверьте изменение
            Console.WriteLine("Modified style font color: " + dxfCollection[0].Font.Color);
            Console.WriteLine("Modified style font bold: " + dxfCollection[0].Font.IsBold);

            // Примените стиль к ячейке, чтобы увидеть эффект
            worksheet.Cells["A1"].PutValue("DxfCollection Property Item Demo");
            worksheet.Cells["A1"].SetStyle(dxfCollection[0]);

            // Сохранить результат
            workbook.Save("DxfCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [Style](../../style/)
* class [DxfCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


