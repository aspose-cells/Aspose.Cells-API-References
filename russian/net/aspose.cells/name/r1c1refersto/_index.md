---
title: "Name.R1C1RefersTo"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Name. Получает или задает ссылку R1C1 для Name"
type: docs
url: /ru/net/aspose.cells/name/r1c1refersto/
---
## Name.R1C1RefersTo property

Получает или задает ссылку R1C1 для [`Name`](../).

```csharp
public string R1C1RefersTo { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyR1C1RefersToDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить новое имя в коллекцию имен
            int nameIndex = workbook.Worksheets.Names.Add("TestRange");
            Name name = workbook.Worksheets.Names[nameIndex];
            
            // Установить ссылку R1C1 для имени
            name.R1C1RefersTo = "'Sheet1'!R3C1:R9C4";
            
            // Проверить, что ссылка установлена корректно
            Console.WriteLine("Name refers to: " + name.RefersTo);
            
            // Сохраните книгу
            workbook.Save("NamePropertyR1C1RefersToDemo_Output.xlsx");
        }
    }
}
```

### См. также

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


