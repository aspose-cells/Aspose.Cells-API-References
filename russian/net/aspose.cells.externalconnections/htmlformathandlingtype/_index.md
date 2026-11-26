---
title: "Перечисление HtmlFormatHandlingType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Перечисление Aspose.Cells.ExternalConnections.HtmlFormatHandlingType. Указывает, как обрабатывать форматирование из HTML‑источника"
type: docs
url: /ru/net/aspose.cells.externalconnections/htmlformathandlingtype/
---
## HtmlFormatHandlingType enumeration

Указывает, как обрабатывать форматирование из HTML‑источника

```csharp
public enum HtmlFormatHandlingType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| All | `0` | Перенести всё HTML‑форматирование в лист вместе с данными. |
| None | `1` | Импортировать данные как неформатированный текст (присвоение типов данных всё равно происходит). |
| Rtf | `2` | Преобразовать HTML‑форматирование в форматирование богатого текста для данных, импортированных в лист. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassHtmlFormatHandlingTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Продемонстрировать все значения перечисления HtmlFormatHandlingType
                HtmlFormatHandlingType allFormatting = HtmlFormatHandlingType.All;
                HtmlFormatHandlingType noFormatting = HtmlFormatHandlingType.None;
                HtmlFormatHandlingType rtfFormatting = HtmlFormatHandlingType.Rtf;

                // Отобразить значения перечисления
                Console.WriteLine("HtmlFormatHandlingType.All: " + allFormatting);
                Console.WriteLine("HtmlFormatHandlingType.None: " + noFormatting);
                Console.WriteLine("HtmlFormatHandlingType.Rtf: " + rtfFormatting);

                // Смоделировать использование этих значений в сценарии
                worksheet.Cells["A1"].PutValue("Format Handling Types:");
                worksheet.Cells["A2"].PutValue("All Formatting");
                worksheet.Cells["A3"].PutValue("No Formatting");
                worksheet.Cells["A4"].PutValue("RTF Formatting");

                // Сохраните книгу
                workbook.Save("HtmlFormatHandlingTypeDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in HtmlFormatHandlingType demo: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


