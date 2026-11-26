---
title: "Перечисление VisibilityType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.VisibilityType. Представляет состояния видимости листа"
type: docs
url: /ru/net/aspose.cells/visibilitytype/
---
## VisibilityType enumeration

Представляет состояния видимости листа.

```csharp
public enum VisibilityType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| Visible | `0` | Указывает, что лист видим. |
| Hidden | `1` | Указывает, что лист скрыт, но может быть показан пользователем через пользовательский интерфейс. |
| VeryHidden | `2` | Указывает, что лист скрыт и не может быть отображён в пользовательском интерфейсе (UI). Это состояние доступно только программно. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VisibilityTypeDemo
    {
        public static void VisibilityTypeExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("NewSheet");
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Установить имя листа
            worksheet.Name = "DemoSheet";

            // Установить видимость листа как Hidden
            worksheet.VisibilityType = VisibilityType.Hidden;

            // Сохраните книгу
            workbook.Save("VisibilityTypeExample.xlsx");

            // Вывести сообщение, указывающее, что процесс завершён
            Console.WriteLine("Workbook saved with the worksheet visibility set to Hidden.");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


