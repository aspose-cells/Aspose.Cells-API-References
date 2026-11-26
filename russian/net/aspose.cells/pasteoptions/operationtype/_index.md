---
title: "PasteOptions.OperationType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PasteOptions. Получает и задает тип операции при вставке диапазона"
type: docs
url: /ru/net/aspose.cells/pasteoptions/operationtype/
---
## PasteOptions.OperationType property

Получает и задает тип операции при вставке диапазона.

```csharp
public PasteOperationType OperationType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PasteOptionsPropertyOperationTypeDemo
    {
        public static void Run()
        {
            // Создайте исходную книгу с образцовыми данными
            Workbook wbOrigin = new Workbook();
            Worksheet sourceSheet = wbOrigin.Worksheets[0];
            sourceSheet.Cells["A1"].PutValue("Source Data");
            sourceSheet.Cells["B2"].PutValue(100);
            
            // Создайте целевую книгу
            Workbook wbDestination = new Workbook();
            Worksheet destSheet = wbDestination.Worksheets[0];
            destSheet.Cells["A1"].PutValue("Destination Data");
            destSheet.Cells["B2"].PutValue(200); // Will be modified by paste operation
            
            // Создать диапазоны для копирования/вставки
            var rangeOrigin = sourceSheet.Cells.CreateRange("A1:B3");
            var rangeDestination = destSheet.Cells.CreateRange("A1:B3");
            
            // Создать параметры вставки с демонстрацией OperationType
            var options = new PasteOptions
            {
                PasteType = PasteType.All,
                OperationType = PasteOperationType.Add // Values will be added (100 + 200 = 300)
            };
            
            // Выполнить операцию копирования/вставки
            rangeDestination.Copy(rangeOrigin, options);
            
            // Проверить результат
            Console.WriteLine("B2 value after paste with Add operation: " + destSheet.Cells["B2"].IntValue);
            
            // Сохранить результат
            wbDestination.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* enum [PasteOperationType](../../pasteoperationtype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


