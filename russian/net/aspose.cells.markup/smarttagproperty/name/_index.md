---
title: "SmartTagProperty.Name"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство SmartTagProperty. Получает и задает имя свойства"
type: docs
url: /ru/net/aspose.cells.markup/smarttagproperty/name/
---
## SmartTagProperty.Name property

Получает и задает имя свойства.

```csharp
public string Name { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Markup;
    using System;
    using System.Reflection;

    public class SmartTagPropertyPropertyNameDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр SmartTagProperty с помощью рефлексии, поскольку конструктор не публичный.
                var property = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Установить свойство Name
                property.Name = "Department";

                // Отобразите текущее значение свойства Name
                Console.WriteLine("SmartTagProperty Name: " + property.Name);

                // Продемонстрируйте изменение свойства Name
                property.Name = "Project";
                Console.WriteLine("Updated SmartTagProperty Name: " + property.Name);

                // Покажите, что свойство можно читать и изменять
                Console.WriteLine("Name property demonstration completed successfully");
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


