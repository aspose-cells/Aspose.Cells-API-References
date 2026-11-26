---
title: "Перечисление SmartTagShowType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.Markup.SmartTagShowType enum. Представляет тип отображения смарт‑тега."
type: docs
url: /ru/net/aspose.cells.markup/smarttagshowtype/
---
## SmartTagShowType enumeration

Представляет тип отображения смарт‑тега.

```csharp
public enum SmartTagShowType
```

### Значения

| Имя | Значение | Описание |
| --- | --- | --- |
| All | `0` | Указывает, что смарт‑теги включены и отображаются |
| NoSmartTagIndicator | `1` | Указывает, что смарт‑теги включены, но индикатор не отображается. |
| None | `2` | Указывает, что смарт‑теги отключены и не отображаются. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class MarkupClassSmartTagShowTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Продемонстрировать все значения перечисления SmartTagShowType
            Console.WriteLine("SmartTagShowType values:");
            Console.WriteLine($"All: {SmartTagShowType.All}");
            Console.WriteLine($"NoSmartTagIndicator: {SmartTagShowType.NoSmartTagIndicator}");
            Console.WriteLine($"None: {SmartTagShowType.None}");

            // Создать и настроить смарт‑тег
            var smartTagCollection = worksheet.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");

            // Установить свойства, которые использовали бы SmartTagShowType (симулировано, так как реальное свойство недоступно)
            Console.WriteLine("\nSmart tag created at A1 with current date");

            // Сохранить с различными сценариями типов отображения
            workbook.Save("SmartTagShowTypeDemo_All.xlsx");
            Console.WriteLine("Workbook saved with default show type (All)");

            // Создать другую рабочую книгу с другим поведением типа отображения
            Workbook workbook2 = new Workbook();
            Worksheet worksheet2 = workbook2.Worksheets[0];
            worksheet2.SmartTagSetting.Add("urn:schemas-microsoft-com:office:smarttags#date");
            Console.WriteLine("\nSecond workbook created with smart tag at B2");

            workbook2.Save("SmartTagShowTypeDemo_None.xlsx");
            Console.WriteLine("Second workbook saved (simulating None behavior)");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


