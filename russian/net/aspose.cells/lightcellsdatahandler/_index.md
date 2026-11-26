---
title: "Интерфейс LightCellsDataHandler"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.LightCellsDataHandler интерфейс. Представляет обработчик данных ячеек для чтения больших файлов электронных таблиц в режиме лёгкого веса."
type: docs
url: /ru/net/aspose.cells/lightcellsdatahandler/
---
## LightCellsDataHandler interface

Представляет обработчик данных ячеек для чтения больших файлов таблиц в режиме облегчённого доступа.

```csharp
public interface LightCellsDataHandler
```

## Методы

| Имя | Описание |
| --- | --- |
| [ProcessCell](../../aspose.cells/lightcellsdatahandler/processcell/)(Cell) | Начинает обработку одной ячейки. |
| [ProcessRow](../../aspose.cells/lightcellsdatahandler/processrow/)(Row) | Начинает обработку одной строки. |
| [StartCell](../../aspose.cells/lightcellsdatahandler/startcell/)(int) | Подготавливает обработку ячейки. |
| [StartRow](../../aspose.cells/lightcellsdatahandler/startrow/)(int) | Подготавливает обработку строки. |
| [StartSheet](../../aspose.cells/lightcellsdatahandler/startsheet/)(Worksheet) | Начинает обработку рабочего листа. |

### Примечания

При чтении книги в этом режиме, [`StartSheet`](./startsheet/) будет проверяться при чтении каждого листа книги. Для одного листа, если [`StartSheet`](./startsheet/) возвращает true, то все данные и свойства строк/ячеек этого листа будут проверяться и обрабатываться реализацией этого интерфейса. Для каждой строки будет вызываться [`StartRow`](./startrow/) для проверки, требуется ли её обработка. Если строка требует обработки, её свойства будут считаны в первую очередь, и пользователь может получить доступ к их свойствам через [`ProcessRow`](./processrow/). Если ячейки строки также нуждаются в обработке, то [`ProcessRow`](./processrow/) должен вернуть true, после чего для каждой существующей ячейки в этой строке будет вызван [`StartCell`](./startcell/) для проверки, нужна ли обработка ячейки. Если ячейка требует обработки, будет вызван [`ProcessCell`](./processcell/) для обработки ячейки реализацией этого интерфейса. Обратите внимание, пользователь должен работать только со значениями и свойствами текущего объекта Row/Cell, предоставленного соответствующим методом. Поскольку данные ячеек читаются из шаблонного файла потоковым способом, большинство остальных объектов могут быть сброшены/обновлены позже после загрузки данных ячеек. Поэтому операции над другими объектами в этой реализации могут не влиять на объекты, существующие в книге. Ещё хуже, такие операции могут привести к несогласованным данным в книге и вызвать непредвиденные проблемы или исключения позже. Таким образом, для всех остальных объектов, таких как фигуры, ширина столбцов и стили, условное форматирование и т.д., пожалуйста, не работайте с ними в методах этой реализации. Вместо этого управляйте ими после того, как книга будет построена.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerDemo : LightCellsDataHandler
    {
        public static void LightCellsDataHandlerExample()
        {
            // Создать книгу и загрузить её с помощью LightCellsDataHandler
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать экземпляр LightCellsDataHandlerDemo
            LightCellsDataHandlerDemo handler = new LightCellsDataHandlerDemo();

            // Установить LightCellsDataHandler для книги
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = handler;

            // Загрузите книгу с указанными параметрами загрузки
            workbook = new Workbook("LargeFile_original.xlsx", loadOptions);

            // Сохранить книгу, чтобы продемонстрировать процесс
            workbook.Save("ProcessedLargeFile.xlsx");
        }

        // Реализовать метод StartSheet
        public bool StartSheet(Worksheet sheet)
        {
            Console.WriteLine("Starting to process sheet: " + sheet.Name);
            return true; // Continue processing
        }

        // Реализовать метод StartRow
        public bool StartRow(int rowIndex)
        {
            Console.WriteLine("Starting to process row: " + rowIndex);
            return true; // Continue processing
        }

        // Реализовать метод ProcessRow
        public bool ProcessRow(Row row)
        {
            Console.WriteLine("Processing row: " + row.Index);
            return true; // Continue processing
        }

        // Реализовать метод StartCell
        public bool StartCell(int columnIndex)
        {
            Console.WriteLine("Starting to process cell in column: " + columnIndex);
            return true; // Continue processing
        }

        // Реализовать метод ProcessCell
        public bool ProcessCell(Cell cell)
        {
            Console.WriteLine("Processing cell: " + cell.Name + " with value: " + cell.StringValue);
            return true; // Continue processing
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


