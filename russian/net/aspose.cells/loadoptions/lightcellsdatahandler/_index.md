---
title: "LoadOptions.LightCellsDataHandler"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Обработчик данных для обработки данных ячеек при чтении файла шаблона"
type: docs
url: /ru/net/aspose.cells/loadoptions/lightcellsdatahandler/
---
## LoadOptions.LightCellsDataHandler property

Обработчик данных для обработки данных ячеек при чтении шаблонного файла.

```csharp
public LightCellsDataHandler LightCellsDataHandler { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyLightCellsDataHandlerDemo
    {
        public static void Run()
        {
            // Создать пользовательский LightCellsDataHandler для обработки данных ячеек
            var dataHandler = new CustomLightCellsDataHandler();
            
            // Создать LoadOptions и установить обработчик данных
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = dataHandler;

            // Загрузить книгу с пользовательским обработчиком
            using (Workbook workbook = new Workbook("sample.xlsx", loadOptions))
            {
                Console.WriteLine("Workbook processed successfully with LightCellsDataHandler");
            }
        }
    }

    public class CustomLightCellsDataHandler : LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet)
        {
            Console.WriteLine($"Processing sheet: {sheet.Name}");
            return true; // Continue processing this sheet
        }

        public bool StartRow(int rowIndex)
        {
            Console.WriteLine($"  Starting row: {rowIndex}");
            return true; // Continue processing this row
        }

        public bool ProcessRow(Row row)
        {
            // Вы можете обработать данные строк здесь при необходимости
            return true;
        }

        public bool StartCell(int columnIndex)
        {
            Console.WriteLine($"    Starting cell at column: {columnIndex}");
            return true; // Continue processing this cell
        }

        public bool ProcessCell(Cell cell)
        {
            Console.WriteLine($"      Cell[{cell.Row},{cell.Column}]: {cell.Value}");
            return true;
        }
    }
}
```

### См. также

* interface [LightCellsDataHandler](../../lightcellsdatahandler/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


