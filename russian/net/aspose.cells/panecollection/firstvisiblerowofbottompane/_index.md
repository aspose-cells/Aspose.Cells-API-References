---
title: "PaneCollection.FirstVisibleRowOfBottomPane"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaneCollection. Получает и задает первую видимую строку нижней области"
type: docs
url: /ru/net/aspose.cells/panecollection/firstvisiblerowofbottompane/
---
## PaneCollection.FirstVisibleRowOfBottomPane property

Получает и задает первую видимую строку нижней панели.

```csharp
public int FirstVisibleRowOfBottomPane { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные, чтобы создать прокручиваемую область
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // Заморозьте области на строке 10 (это создаст верхнюю и нижнюю области)
            worksheet.FreezePanes(10, 0, 10, 0);
            
            // Получить коллекцию областей
            PaneCollection panes = worksheet.GetPanes();
            
            // Установить первую видимую строку нижней области
            panes.FirstVisibleRowOfBottomPane = 15;
            
            // Вывести первую видимую строку нижней области
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            
            // Сохраните книгу
            workbook.Save("PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo.xlsx");
        }
    }
}
```

### См. также

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


