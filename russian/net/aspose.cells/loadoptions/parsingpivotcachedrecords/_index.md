---
title: "LoadOptions.ParsingPivotCachedRecords"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство LoadOptions. Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. Значение по умолчанию — false"
type: docs
url: /ru/net/aspose.cells/loadoptions/parsingpivotcachedrecords/
---
## LoadOptions.ParsingPivotCachedRecords property

Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. Значение по умолчанию — false.

```csharp
public bool ParsingPivotCachedRecords { get; set; }
```

### Примечания

Применяется только к файлам Excel Xlsx, Xltx, Xltm, Xlsm и xlsb

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyParsingPivotCachedRecordsDemo
    {
        public static void Run()
        {
            // Создать параметры загрузки CSV
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
            
            // Включить разбор кэшированных записей сводных таблиц
            loadOptions.ParsingPivotCachedRecords = true;
            
            // Загрузите книгу с параметрами
            Workbook workbook = new Workbook("example.csv", loadOptions);
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "PivotData";
            
            // Создать сводную таблицу (демонстрируя, что свойство установлено)
            int pivotIndex = worksheet.PivotTables.Add("A1:C10", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Сохраните книгу
            workbook.Save("PivotTableOutput.xlsx");
        }
    }
}
```

### См. также

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


