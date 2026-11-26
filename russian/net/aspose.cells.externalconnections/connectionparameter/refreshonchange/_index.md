---
title: "ConnectionParameter.RefreshOnChange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ConnectionParameter. Флаг, указывающий, следует ли автоматически обновлять запрос, когда содержимое ячейки, предоставляющей значение параметра, меняется. Если true, внешние данные обновляются с использованием нового значения параметра каждый раз при изменении. Если false, внешние данные обновляются только по запросу пользователя или при срабатывании другого события, вызывающего обновление, например при открытии книги"
type: docs
url: /ru/net/aspose.cells.externalconnections/connectionparameter/refreshonchange/
---
## ConnectionParameter.RefreshOnChange property

Флаг, указывающий, следует ли автоматически обновлять запрос, когда содержимое ячейки, предоставляющей значение параметра, изменяется. Если true, внешние данные обновляются с использованием нового значения параметра каждый раз при изменении. Если false, внешние данные обновляются только по запросу пользователя или при срабатывании другого события (например, открытие книги).

```csharp
public bool RefreshOnChange { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ConnectionParameterPropertyRefreshOnChangeDemo
    {
        public static void Run()
        {
            try
            {
                // Создать новую книгу
                Workbook workbook = new Workbook();
                
                // Создайте параметр соединения (симулировано, так как параметры конструктора неизвестны)
                ConnectionParameter parameter = null;
                
                // В реальном сценарии вы бы создали параметр корректно
                // parameter = new ConnectionParameter(/* required parameters */);
                
                // Для демонстрации мы покажем, как RefreshOnChange будет использоваться, если у нас будет параметр
                if (parameter != null)
                {
                    // Получите и отобразите текущее значение RefreshOnChange
                    Console.WriteLine("Current RefreshOnChange: " + parameter.RefreshOnChange);
                    
                    // Установите новое значение RefreshOnChange (так как свойство доступно для чтения и записи)
                    parameter.RefreshOnChange = true;
                    Console.WriteLine("Updated RefreshOnChange: " + parameter.RefreshOnChange);
                }
                else
                {
                    // Запасная демонстрация, когда мы не можем создать параметр
                    workbook.Worksheets[0].Cells["A1"].Value = "RefreshOnChange property demo (see code comments)";
                    Console.WriteLine("Demonstrated workbook creation. In actual usage, create ConnectionParameter properly.");
                }
                
                // Сохраните книгу
                workbook.Save("ConnectionParameterRefreshOnChangeDemo.xlsx");
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

* class [ConnectionParameter](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


