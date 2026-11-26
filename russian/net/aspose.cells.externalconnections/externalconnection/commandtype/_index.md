---
title: "ExternalConnection.CommandType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ExternalConnection. Указывает тип команды OLE DB. 1. Запрос указывает имя куба 2. Запрос указывает SQL‑оператор 3. Запрос указывает имя таблицы 4. Запрос указывает, что предоставлена информация по умолчанию, и интерпретация зависит от поставщика 5. Запрос выполняется к веб‑основному поставщику List Data Provider"
type: docs
url: /ru/net/aspose.cells.externalconnections/externalconnection/commandtype/
---
## ExternalConnection.CommandType property

Указывает тип команды OLE DB. 1. Запрос указывает имя куба 2. Запрос указывает SQL‑оператор 3. Запрос указывает имя таблицы 4. Запрос указывает, что предоставлена информация по умолчанию, и интерпретация зависит от поставщика. 5. Запрос направлен к веб‑ориентированному List Data Provider.

```csharp
public virtual OLEDBCommandType CommandType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.ExternalConnections;

namespace AsposeCellsExamples
{
    public class ExternalConnectionPropertyCommandTypeDemo
    {
        public static void Run()
        {
            // Создайте книгу с примерными данными
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте примерные данные
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1500);

            // Создайте сводную таблицу
            int index = worksheet.PivotTables.Add("A1:B3", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];

            // Получить внешнее соединение
            ExternalConnection conn = pivotTable.GetSourceDataConnections()[0];
            
            // Продемонстрировать свойство CommandType
            Console.WriteLine("Original CommandType: " + conn.CommandType);
            
            // Изменить и показать CommandType
            conn.CommandType = Aspose.Cells.ExternalConnections.OLEDBCommandType.TableName;
            Console.WriteLine("Modified CommandType: " + conn.CommandType);
            
            // Сохраните книгу
            workbook.Save("ExternalConnectionCommandTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [OLEDBCommandType](../../oledbcommandtype/)
* class [ExternalConnection](../)
* namespace [Aspose.Cells.ExternalConnections](../../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../../)


