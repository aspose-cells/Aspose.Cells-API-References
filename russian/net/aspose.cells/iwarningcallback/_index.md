---
title: "Интерфейс IWarningCallback"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Интерфейс Aspose.Cells.IWarningCallback. Интерфейс обратного вызова предупреждения"
type: docs
url: /ru/net/aspose.cells/iwarningcallback/
---
## IWarningCallback interface

Интерфейс обратного вызова предупреждения.

```csharp
public interface IWarningCallback
```

## Методы

| Имя | Описание |
| --- | --- |
| [Warning](../../aspose.cells/iwarningcallback/warning/)(WarningInfo) | Наш обратный вызов должен реализовать только метод "Warning". |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IWarningCallbackDemo : IWarningCallback
    {
        // Реализация метода Warning из интерфейса IWarningCallback
        public void Warning(WarningInfo warningInfo)
        {
            // Отобразить сообщение предупреждения
            Console.WriteLine("Warning: " + warningInfo.WarningType + " - " + warningInfo.Description);
        }

        public static void IWarningCallbackExample()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Установить обратный вызов предупреждения
            workbook.Settings.WarningCallback = new IWarningCallbackDemo();

            // Загрузить книгу с потенциальными предупреждениями
            try
            {
                workbook = new Workbook("example.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception: " + ex.Message);
            }

            // Сохраните книгу
            workbook.Save("IWarningCallbackExample.xlsx");
        }
    }

}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


