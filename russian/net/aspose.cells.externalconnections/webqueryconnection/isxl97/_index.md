---
title: "WebQueryConnection.IsXl97"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство WebQueryConnection. Этот флаг существует для обратной совместимости со старыми существующими файлами электронных таблиц и устанавливается в true, если этот веб‑запрос был создан в Microsoft Excel 97. Это необязательный атрибут, который можно игнорировать"
type: docs
url: /ru/net/aspose.cells.externalconnections/webqueryconnection/isxl97/
---
## WebQueryConnection.IsXl97 property

Этот флаг существует для обеспечения обратной совместимости со старыми существующими файлами электронных таблиц и устанавливается в true, если этот веб‑запрос был создан в Microsoft Excel 97. Это необязательный атрибут, который можно игнорировать.

```csharp
public bool IsXl97 { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class WebQueryConnectionPropertyIsXl97Demo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Создайте лист с некоторыми данными, чтобы пример имел смысл
                Worksheet worksheet = workbook.Worksheets[0];
                worksheet.Cells["A1"].Value = "Sample Data";
                
                // Создайте соединение веб‑запроса, загрузив его из существующего файла или создав правильно
                // Поскольку мы не можем создать WebQueryConnection напрямую, мы получим доступ к существующему объекту
                if (workbook.DataConnections.Count > 0 && 
                    workbook.DataConnections[0] is WebQueryConnection connection)
                {
                    // Отобразите начальное значение IsXl97
                    Console.WriteLine("Initial IsXl97 value: " + connection.IsXl97);
                    
                    // Установите IsXl97 в true (поскольку он доступен для чтения и записи)
                    connection.IsXl97 = true;
                    Console.WriteLine("Updated IsXl97 value: " + connection.IsXl97);
                    
                    // Установите IsXl97 обратно в false
                    connection.IsXl97 = false;
                    Console.WriteLine("Final IsXl97 value: " + connection.IsXl97);
                    
                    // Сохраните книгу
                    workbook.Save("WebQueryConnectionIsXl97Demo.xlsx");
                }
                else
                {
                    Console.WriteLine("No web query connections found in the workbook.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [WebQueryConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


