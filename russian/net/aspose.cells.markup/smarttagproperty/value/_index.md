---
title: "SmartTagProperty.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SmartTagProperty. Получает и задает значение свойства"
type: docs
url: /ru/net/aspose.cells.markup/smarttagproperty/value/
---
## SmartTagProperty.Value property

Получает и задает значение свойства.

```csharp
public string Value { get; set; }
```

### Примеры

```csharp
using Aspose.Cells.Markup;
using System;

namespace AsposeCellsExamples
{
    public class SmartTagPropertyPropertyValueDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр SmartTagProperty, используя непубличный конструктор
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Установите имя и значение свойства
                property.Name = "Category";
                property.Value = "Finance";

                // Отобразите значения свойств
                Console.WriteLine($"SmartTagProperty Name : {property.Name}");
                Console.WriteLine($"SmartTagProperty Value: {property.Value}");
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

* class [SmartTagProperty](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


