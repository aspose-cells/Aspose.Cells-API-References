---
title: "Класс XmlDataBinding"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.XmlDataBinding класс. Представляет информацию о привязке XML‑данных"
type: docs
url: /ru/net/aspose.cells/xmldatabinding/
---
## XmlDataBinding class

Представляет информацию о привязке данных Xml.

```csharp
public class XmlDataBinding
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Url](../../aspose.cells/xmldatabinding/url/) { get; } | Получает URL источника этой привязки данных. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellsClassXmlDataBindingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать объект списка, который будет использовать привязку XML‑данных
            ListObject listObject = worksheet.ListObjects[worksheet.ListObjects.Add(0, 0, 5, 4, true)];

            // Получить информацию о привязке XML‑данных (обычно задаётся при импорте XML‑данных)
            XmlDataBinding xmlDataBinding = listObject.XmlMap.DataBinding;

            // Отобразить URL XML‑источника данных (свойство только для чтения)
            Console.WriteLine("XML Data Binding Source URL: " + xmlDataBinding.Url);

            // Примечание: В реальном сценарии URL будет установлен при импорте XML-данных
            // В демонстрационных целях мы показываем, как получить доступ к свойству

            // Сохраните книгу
            workbook.Save("XmlDataBindingDemo.xlsx");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


