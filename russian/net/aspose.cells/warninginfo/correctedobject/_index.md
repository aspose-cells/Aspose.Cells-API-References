---
title: "WarningInfo.CorrectedObject"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WarningInfo. Получает и задает исправленный объект"
type: docs
url: /ru/net/aspose.cells/warninginfo/correctedobject/
---
## WarningInfo.CorrectedObject property

Получает и задает исправленный объект.

```csharp
public object CorrectedObject { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WarningInfoPropertyCorrectedObjectDemo
    {
        public static void Run()
        {
            // Создайте книгу и вызовите предупреждение
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите имя, которое обычно вызывает предупреждение
            string originalName = "MyRange";
            worksheet.Cells.CreateRange(originalName);
            
            // Обработать обратный вызов предупреждения
            workbook.Settings.WarningCallback = new WarningHandler();
            
            // Эта операция вызовет обратный вызов предупреждения
            worksheet.Cells.CreateRange(originalName); // Duplicate range name
        }
    }

    public class WarningHandler : IWarningCallback
    {
        public void Warning(WarningInfo warningInfo)
        {
            if (warningInfo.WarningType == WarningType.DuplicateDefinedName)
            {
                // Продемонстрировать использование CorrectedObject
                warningInfo.CorrectedObject = "_" + warningInfo.ErrorObject;
                Console.WriteLine($"Warning handled. Original: {warningInfo.ErrorObject}, Corrected: {warningInfo.CorrectedObject}");
            }
        }
    }
}
```

### См. также

* class [WarningInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


