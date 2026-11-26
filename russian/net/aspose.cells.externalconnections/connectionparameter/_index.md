---
title: "Класс ConnectionParameter"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.ExternalConnections.ConnectionParameter. Указывает свойства любых параметров, используемых во внешних соединениях данных. Параметры действительны для ODBC и веб‑запросов."
type: docs
url: /ru/net/aspose.cells.externalconnections/connectionparameter/
---
## ConnectionParameter class

Указывает свойства любых параметров, используемых во внешних соединениях данных. Параметры действительны для ODBC и веб‑запросов.

```csharp
public class ConnectionParameter
```

## Свойства

| Имя | Описание |
| --- | --- |
| [CellReference](../../aspose.cells.externalconnections/connectionparameter/cellreference/) { get; set; } | Ссылка на ячейку, указывающая, значение какой ячейки использовать для параметра запроса. Используется только когда parameterType имеет значение cell. |
| [Name](../../aspose.cells.externalconnections/connectionparameter/name/) { get; set; } | Имя параметра. |
| [Prompt](../../aspose.cells.externalconnections/connectionparameter/prompt/) { get; set; } | Строка подсказки для параметра. Предоставляется пользователю таблицы вместе с пользовательским интерфейсом ввода для сбора значения параметра перед обновлением внешних данных. Используется только когда parameterType = prompt. |
| [RefreshOnChange](../../aspose.cells.externalconnections/connectionparameter/refreshonchange/) { get; set; } | Флаг, указывающий, следует ли автоматически обновлять запрос, когда содержимое ячейки, предоставляющей значение параметра, изменяется. Если true, внешние данные обновляются с использованием нового значения параметра каждый раз при изменении. Если false, внешние данные обновляются только по запросу пользователя или при срабатывании другого события (например, открытие книги). |
| [SqlType](../../aspose.cells.externalconnections/connectionparameter/sqltype/) { get; set; } | SQL‑тип данных параметра. Действителен только для источников ODBC. |
| [Type](../../aspose.cells.externalconnections/connectionparameter/type/) { get; set; } | Тип используемого параметра. Если parameterType=value, будет использовано значение из boolean, double, integer или string. В этом случае ожидается, что будет указано только одно из {boolean, double, integer, or string}. |
| [Value](../../aspose.cells.externalconnections/connectionparameter/value/) { get; set; } | Нецелочисленное числовое значение, целочисленное значение, строковое значение или логическое значение, используемое в качестве параметра запроса. Используется только когда parameterType имеет значение value. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassConnectionParameterDemo
    {
        public static void Run()
        {
            // Создать новую книгу для демонстрации
            Workbook workbook = new Workbook();
            
            try
            {
                // Создать параметр соединения с помощью рефлексии, поскольку конструктор не является публичным
                ConnectionParameter parameter = (ConnectionParameter)Activator.CreateInstance(typeof(ConnectionParameter), nonPublic: true);
                
                // Установите базовые свойства
                parameter.Name = "CustomerID";
                parameter.Type = ConnectionParameterType.Value;
                parameter.Value = "CUST1001";
                parameter.RefreshOnChange = true;
                parameter.Prompt = "Enter Customer ID:";
                
                // Отобразить информацию о параметре
                Console.WriteLine($"Created parameter: {parameter.Name}");
                Console.WriteLine($"Type: {parameter.Type}");
                Console.WriteLine($"Value: {parameter.Value}");
                Console.WriteLine($"Refresh on change: {parameter.RefreshOnChange}");
                Console.WriteLine($"Prompt: {parameter.Prompt}");
                
                // Сохраните книгу
                workbook.Save("ConnectionParameterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ConnectionParameter: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


