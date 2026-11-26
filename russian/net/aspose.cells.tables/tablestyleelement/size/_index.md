---
title: "TableStyleElement.Size"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство TableStyleElement. Количество строк или столбцов в одной полосе чередования. Применяется только когда тип — firstRowStripe, secondRowStripe, firstColumnStripe или secondColumnStripe."
type: docs
url: /ru/net/aspose.cells.tables/tablestyleelement/size/
---
## TableStyleElement.Size property

Количество строк или столбцов в одной полосе чередования. Применяется только когда тип — firstRowStripe, secondRowStripe, firstColumnStripe или secondColumnStripe.

```csharp
public int Size { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleElementPropertySizeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте примерные данные для создания таблицы
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    worksheet.Cells[i, j].PutValue($"Data {i},{j}");
                }
            }

            // Создать таблицу
            int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = TableStyleType.TableStyleMedium9;

            // Создать стиль таблицы, используя коллекцию стилей рабочей книги
            TableStyleCollection styleCollection = workbook.Worksheets.TableStyles;
            int styleIndex = styleCollection.AddTableStyle("CustomStyle");
            TableStyle style = styleCollection[styleIndex];
            table.TableStyleName = style.Name;

            // Добавить элементы полосы для демонстрации свойства Size
            style.TableStyleElements.Add(TableStyleElementType.FirstRowStripe);
            style.TableStyleElements.Add(TableStyleElementType.SecondRowStripe);

            // Получить доступ к элементам полосы
            TableStyleElement firstStripe = style.TableStyleElements[TableStyleElementType.FirstRowStripe];
            TableStyleElement secondStripe = style.TableStyleElements[TableStyleElementType.SecondRowStripe];

            // Отобразить текущие значения Size
            Console.WriteLine("Initial First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Initial Second Stripe Size: " + secondStripe.Size);

            // Изменить размеры полос
            firstStripe.Size = 2;
            secondStripe.Size = 3;

            // Отобразить изменённые значения
            Console.WriteLine("Modified First Stripe Size: " + firstStripe.Size);
            Console.WriteLine("Modified Second Stripe Size: " + secondStripe.Size);

            // Сохраните книгу, чтобы увидеть эффекты
            workbook.Save("TableStyleElementSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


