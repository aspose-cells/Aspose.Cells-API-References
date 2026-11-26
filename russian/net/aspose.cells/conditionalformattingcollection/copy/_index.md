---
title: "ConditionalFormattingCollection.Copy"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ConditionalFormattingCollection. Копирует условное форматирование"
type: docs
url: /ru/net/aspose.cells/conditionalformattingcollection/copy/
---
## ConditionalFormattingCollection.Copy method

Копирует условное форматирование.

```csharp
public void Copy(ConditionalFormattingCollection cfs)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cfs | ConditionalFormattingCollection | Условное форматирование |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingCollectionMethodCopyWithConditionalFormattingCollectioDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook destWorkbook = new Workbook();
            Worksheet destSheet = destWorkbook.Worksheets[0];

            // Создать исходную книгу с условным форматированием
            Workbook sourceWorkbook = new Workbook();
            Worksheet sourceSheet = sourceWorkbook.Worksheets[0];

            // Добавить пример условного форматирования на исходный лист
            int index = sourceSheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sourceSheet.ConditionalFormattings[index];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
            
            // Создать и применить стиль к условию форматирования
            Style style = sourceWorkbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.Red;
            FormatCondition fc = fcc[0];
            fc.Style = style;

            // Применить к диапазону
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 5;
            area.StartColumn = 0;
            area.EndColumn = 5;
            fcc.AddArea(area);

            // Копировать условное форматирование из источника в назначение
            destSheet.ConditionalFormattings.Copy(sourceSheet.ConditionalFormattings);

            // Сохраните книгу
            destWorkbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [ConditionalFormattingCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


