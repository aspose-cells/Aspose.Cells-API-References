---
title: "XlsSaveOptions.LightCellsDataProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XlsSaveOptions. Поставщик данных для сохранения книги в лёгком режиме"
type: docs
url: /ru/net/aspose.cells/xlssaveoptions/lightcellsdataprovider/
---
## XlsSaveOptions.LightCellsDataProvider property

Поставщик данных для сохранения книги в лёгком режиме.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Создайте параметры сохранения XLS
            XlsSaveOptions saveOptions = new XlsSaveOptions();
            
            // Установите LightCellsDataProvider
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();
            
            // Сохраните книгу в режиме LightCells
            workbook.Save("output.xls", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        public bool IsGatherString()
        {
            return true;
        }

        public int NextCell()
        {
            return 0; // Only process first cell for demonstration
        }

        public int NextRow()
        {
            return 0; // Only process first row for demonstration
        }

        public void StartCell(Cell cell)
        {
            // Установите длинное строковое значение для демонстрации обработки LightCells
            cell.PutValue(new string('X', 257));
        }

        public void StartRow(Row row)
        {
            // Для этой демонстрации особая обработка строк не требуется
        }

        public bool StartSheet(int sheetIndex)
        {
            // Для этой демонстрации особая обработка листов не требуется
            return false;
        }
    }
}
```

### См. также

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


