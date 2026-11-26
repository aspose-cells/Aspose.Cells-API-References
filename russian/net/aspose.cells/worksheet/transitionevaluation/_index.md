---
title: "Worksheet.TransitionEvaluation"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Worksheet property. Указывает, включена ли опция совместимости Lotus для оценки переходных формул"
type: docs
url: /ru/net/aspose.cells/worksheet/transitionevaluation/
---
## Worksheet.TransitionEvaluation property

Указывает, включена ли опция Transition Formula Evaluation (совместимость с Lotus).

```csharp
public bool TransitionEvaluation { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyTransitionEvaluationDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установите свойство TransitionEvaluation
            worksheet.TransitionEvaluation = true;
            
            // Отобразить значение свойства
            Console.WriteLine("TransitionEvaluation: " + worksheet.TransitionEvaluation);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            // Загрузить сохранённую книгу, чтобы проверить свойство
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            Console.WriteLine("Loaded TransitionEvaluation: " + loadedWorksheet.TransitionEvaluation);
        }
    }
}
```

### См. также

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


