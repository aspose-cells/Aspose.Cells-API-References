---
title: "WebQueryConnection.HtmlFormat"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebQueryConnection. Как обрабатывать форматирование из HTML‑источника при импорте данных веб‑запроса в лист. Актуально, когда sourceData равно True"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/htmlformat/
---
## WebQueryConnection.HtmlFormat property

Как обрабатывать форматирование из HTML‑источника при импорте данных веб‑запроса в лист. Актуально, когда sourceData равно True.

```csharp
public HtmlFormatHandlingType HtmlFormat { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyHtmlFormatDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получите первое существующее подключение веб‑запроса (если есть)
            // Или создайте новое, загрузив файл с веб‑подключениями
            if (workbook.DataConnections.Count > 0)
            {
                try
                {
                    WebQueryConnection connection = (WebQueryConnection)workbook.DataConnections[0];
                    
                    // Отобразите начальное значение HtmlFormat
                    Console.WriteLine("Initial HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Установите HtmlFormat в Rtf (демонстрация операции записи)
                    connection.HtmlFormat = HtmlFormatHandlingType.Rtf;
                    Console.WriteLine("Updated HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Установите HtmlFormat в None
                    connection.HtmlFormat = HtmlFormatHandlingType.None;
                    Console.WriteLine("Final HtmlFormat value: " + connection.HtmlFormat);
                    
                    // Сохраните книгу с подключением веб‑запроса
                    workbook.Save("WebQueryConnectionHtmlFormatDemo.xlsx");
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Error: {ex.Message}");
                }
            }
            else
            {
                Console.WriteLine("No web query connections found in the workbook.");
            }
        }
    }
}
```

### См. также

* enum [HtmlFormatHandlingType](../../htmlformathandlingtype/)
* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


