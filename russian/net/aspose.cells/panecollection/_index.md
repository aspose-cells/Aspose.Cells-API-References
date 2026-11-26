---
title: "Класс PaneCollection"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.PaneCollection. Представляет все объекты Pane, отображаемые в указанном окне"
type: docs
url: /ru/net/aspose.cells/panecollection/
---
## PaneCollection class

Представляет все объекты Pane, отображаемые в указанном окне.

```csharp
public class PaneCollection
```

## Свойства

| Имя | Описание |
| --- | --- |
| [AcitvePaneType](../../aspose.cells/panecollection/acitvepanetype/) { get; set; } | (**Obsolete.**) Получает и задает активную панель. |
| [ActivePaneType](../../aspose.cells/panecollection/activepanetype/) { get; set; } | Получает и задает активную панель. |
| [FirstVisibleColumnOfRightPane](../../aspose.cells/panecollection/firstvisiblecolumnofrightpane/) { get; set; } | Получает и задает первый видимый столбец правой панели. |
| [FirstVisibleRowOfBottomPane](../../aspose.cells/panecollection/firstvisiblerowofbottompane/) { get; set; } | Получает и задает первую видимую строку нижней панели. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPaneCollectionDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].Value = $"Row {i}, Col {j}";
                }
            }
            
            // Заморозить панели на строке 5, столбце 1
            sheet.FreezePanes(5, 1, 5, 1);
            
            // Получить коллекцию панелей
            PaneCollection panes = sheet.GetPanes();
            
            // Изменить настройки панелей
            panes.FirstVisibleRowOfBottomPane = 5;
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Сохраните книгу
            workbook.Save("PaneCollectionDemo.xls", SaveFormat.Excel97To2003);
            
            Console.WriteLine("PaneCollection demo executed successfully.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


