---
title: "XlsbSaveOptions.LightCellsDataProvider"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XlsbSaveOptions. Поставщик данных для сохранения книги в легком режиме"
type: docs
url: /ru/net/aspose.cells/xlsbsaveoptions/lightcellsdataprovider/
---
## XlsbSaveOptions.LightCellsDataProvider property

Поставщик данных для сохранения книги в лёгком режиме.

```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```

### Примеры

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XlsbSaveOptionsPropertyLightCellsDataProviderDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Заполните некоторыми образцовыми данными
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Data {i}");
            }

            // Создать параметры сохранения XLSB
            XlsbSaveOptions saveOptions = new XlsbSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            // Сохранить книгу с LightCellsDataProvider
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // Проверить сохранённые данные
                stream.Seek(0, SeekOrigin.Begin);
                Workbook savedWorkbook = new Workbook(stream);
                Console.WriteLine("Workbook saved successfully with LightCellsDataProvider");
            }
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
            // Реализуйте логику итерации ячеек здесь
            return -1; // Return -1 when no more cells
        }

        public int NextRow()
        {
            // Реализуйте логику итерации строк здесь
            return -1; // Return -1 when no more rows
        }

        public void StartCell(Cell cell)
        {
            // Реализуйте логику обработки ячеек здесь
        }

        public void StartRow(Row row)
        {
            // Реализуйте логику обработки строк здесь
        }

        public bool StartSheet(int sheetIndex)
        {
            // Реализуйте логику обработки листов здесь
            return true; // Return true to process the sheet
        }
    }
}
```

### См. также

* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


