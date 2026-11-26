---
title: "PaneCollection.FirstVisibleColumnOfRightPane"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PaneCollection. Получает и задает первую видимую колонку правой области"
type: docs
url: /ru/net/aspose.cells/panecollection/firstvisiblecolumnofrightpane/
---
## PaneCollection.FirstVisibleColumnOfRightPane property

Получает и задает первый видимый столбец правой панели.

```csharp
public int FirstVisibleColumnOfRightPane { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleColumnOfRightPaneDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Заморозьте области, указав индексы строки и столбца (5, 3)
            sheet.FreezePanes(5, 3, 5, 3);
            
            // Получить коллекцию областей
            PaneCollection panes = sheet.GetPanes();
            
            // Установить первую видимую колонку правой области
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Сохраните книгу
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### См. также

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


