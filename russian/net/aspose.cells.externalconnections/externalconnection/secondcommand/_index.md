---
title: "ExternalConnection.SecondCommand"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Указывает строку текста второй команды, которая сохраняется, когда используются серверные поля страниц PivotTable. Для ODBC‑соединений serverCommand обычно представляет более широкий запрос, чем command, без условия WHERE в первом. На основе этих двух параметров commandsCommand и ServerCommand UI может быть заполнен, и могут быть построены параметризованные запросы."
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/secondcommand/
---
## ExternalConnection.SecondCommand property

Указывает вторую строку команды, которая сохраняется, когда используются полевые элементы PivotTable на основе сервера. Для ODBC‑подключений serverCommand обычно представляет более широкий запрос, чем command (в первом нет предложения WHERE). На основе этих двух команд (Command и ServerCommand) можно заполнить пользовательский интерфейс параметров и построить параметризованные запросы.

```csharp
public virtual string SecondCommand { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionPropertySecondCommandDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            try
            {
                // Получить доступ к первому внешнему соединению (при условии, что оно существует)
                ExternalConnection connection = workbook.DataConnections[0];
                
                // Отобразить текущее значение SecondCommand (операция чтения)
                Console.WriteLine("Initial SecondCommand value: " + connection.SecondCommand);
                
                // Установить новое значение SecondCommand (поскольку оно доступно для чтения и записи)
                connection.SecondCommand = "SELECT * FROM Customers WHERE Country = 'USA'";
                Console.WriteLine("Updated SecondCommand value: " + connection.SecondCommand);
                
                // Очистить SecondCommand, чтобы продемонстрировать установку пустой строки
                connection.SecondCommand = string.Empty;
                Console.WriteLine("Cleared SecondCommand value: " + connection.SecondCommand);
                
                // Сохранить книгу с изменёнными настройками соединения
                workbook.Save("SecondCommandDemo.xlsx");
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

* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


