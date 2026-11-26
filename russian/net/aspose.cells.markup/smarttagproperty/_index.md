---
title: "Класс SmartTagProperty"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Markup.SmartTagProperty класс. Представляет свойство смарт‑тега ячейки."
type: docs
url: /ru/net/aspose.cells.markup/smarttagproperty/
---
## SmartTagProperty class

Представляет свойство смарт‑тега ячейки.

```csharp
public class SmartTagProperty
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Name](../../aspose.cells.markup/smarttagproperty/name/) { get; set; } | Получает и задает имя свойства. |
| [Value](../../aspose.cells.markup/smarttagproperty/value/) { get; set; } | Получает и задает значение свойства. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagPropertyDemo
    {
        public static void Run()
        {
            try
            {
                // Создайте экземпляр SmartTagProperty с помощью рефлексии, поскольку конструктор не публичный.
                var smartTagProperty = (SmartTagProperty)Activator.CreateInstance(typeof(SmartTagProperty), true);

                // Установите свойства Name и Value
                smartTagProperty.Name = "DocumentType";
                smartTagProperty.Value = "FinancialReport";

                // Отобразите значения свойств
                Console.WriteLine($"SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"SmartTagProperty Value: {smartTagProperty.Value}");

                // Продемонстрировать изменение свойств
                smartTagProperty.Name = "Status";
                smartTagProperty.Value = "Approved";

                Console.WriteLine($"Updated SmartTagProperty Name: {smartTagProperty.Name}");
                Console.WriteLine($"Updated SmartTagProperty Value: {smartTagProperty.Value}");

                Console.WriteLine("SmartTagProperty demonstration completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SmartTagProperty: {ex.Message}");
            }
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


