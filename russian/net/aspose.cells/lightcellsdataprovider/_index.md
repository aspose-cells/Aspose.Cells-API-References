---
title: "Интерфейс LightCellsDataProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Интерфейс Aspose.Cells.LightCellsDataProvider. Представляет поставщик данных для сохранения больших файлов электронных таблиц в облегчённом режиме."
type: docs
url: /ru/net/aspose.cells/lightcellsdataprovider/
---
## LightCellsDataProvider interface

Представляет поставщик данных для сохранения больших файлов таблиц в режиме облегчённого доступа.

```csharp
public interface LightCellsDataProvider
```

## Методы

| Имя | Описание |
| --- | --- |
| [IsGatherString](../../aspose.cells/lightcellsdataprovider/isgatherstring/)() | Проверяет, нужно ли текущое строковое значение ячейки собрать в глобальный пул. |
| [NextCell](../../aspose.cells/lightcellsdataprovider/nextcell/)() | Получает следующую ячейку для сохранения. |
| [NextRow](../../aspose.cells/lightcellsdataprovider/nextrow/)() | Получает следующую строку для сохранения. |
| [StartCell](../../aspose.cells/lightcellsdataprovider/startcell/)(Cell) | Начинает сохранять данные одной ячейки. |
| [StartRow](../../aspose.cells/lightcellsdataprovider/startrow/)(Row) | Начинает сохранять данные одной строки. |
| [StartSheet](../../aspose.cells/lightcellsdataprovider/startsheet/)(int) | Начинает сохранять лист. |

### Примечания

При сохранении книги в этом режиме, [`StartSheet`](./startsheet/) будет проверяться при сохранении каждого листа в книге. Для одного листа, если [`StartSheet`](./startsheet/) возвращает true, то все данные и свойства, которые должны быть сохранены для строк/ячеек этого листа, будут предоставлены реализацией этого интерфейса. Сначала будет вызван [`NextRow`](./nextrow/) для получения индекса следующей строки, которую нужно сохранить. Если возвращён действительный индекс строки (индекс строки должен быть в возрастающем порядке для сохраняемых строк), то объект Row, представляющий эту строку, будет предоставлен через [`StartRow`](./startrow/) для установки его свойств. Для одной строки сначала проверяется [`NextCell`](./nextcell/). Если возвращён действительный индекс столбца (индекс столбца должен быть в возрастающем порядке для всех ячеек текущей строки), то объект Cell, представляющий эту ячейку, будет предоставлен через [`StartCell`](./startcell/) для установки его данных и свойств. После [`StartCell`](./startcell/) ячейка будет сохранена напрямую в результирующий файл таблицы. Затем будет проверена и обработана следующая ячейка.  Обратите внимание, пользователь должен обновлять только значения и свойства текущего объекта Row/Cell, предоставленного соответствующим методом. Поскольку данные ячеек записываются в результирующий файл потоковым способом, большинство других объектов уже могли быть записаны в файл или собраны и записаны как глобальные данные для них. Поэтому при обновлении других объектов во время сохранения данных ячеек такие операции могут не повлиять на сохраняемые данные. Ещё хуже, эти операции могут привести к сохранению несогласованных данных в результирующий файл и в конечном итоге повредить файл. Поэтому для всех остальных объектов, таких как фигуры, ширина столбцов и стили, условное форматирование и т.д., пожалуйста, не изменяйте их в каких-либо методах этой реализации. Вместо этого управлять ими и привести к окончательному состоянию следует до вызова метода "Save" книги.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderDemo
    {
        public static void LightCellsDataProviderExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте пользовательский LightCellsDataProvider
            CustomLightCellsDataProvider dataProvider = new CustomLightCellsDataProvider();

            // Установите LightCellsDataProvider для сохранения книги
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx)
            {
                LightCellsDataProvider = dataProvider
            };

            // Сохраните книгу с пользовательским LightCellsDataProvider
            workbook.Save("LightCellsDataProviderExample.xlsx", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private int currentRow = -1;
        private int currentCell = -1;

        public bool StartSheet(int sheetIndex)
        {
            // Начните обработку первого листа
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            // Перейдите к следующей строке
            currentRow++;
            currentCell = -1;

            // Верните текущий индекс строки или -1, если строк больше нет
            return currentRow < 10 ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // Инициализируйте строку при необходимости
        }

        public int NextCell()
        {
            // Перейдите к следующей ячейке
            currentCell++;

            // Верните текущий индекс ячейки или -1, если ячеек больше нет
            return currentCell < 10 ? currentCell : -1;
        }

        public void StartCell(Cell cell)
        {
            // Установить значение ячейки
            cell.PutValue($"R{currentRow}C{currentCell}");
        }

        public bool IsGatherString()
        {
            // Верните, следует ли собирать строки в глобальный пул
            return false;
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


