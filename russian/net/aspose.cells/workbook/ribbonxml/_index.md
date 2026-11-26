---
title: "Workbook.RibbonXml"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Workbook. Получает и задает XML‑файл, определяющий пользовательский интерфейс Ribbon"
type: docs
url: /ru/net/aspose.cells/workbook/ribbonxml/
---
## Workbook.RibbonXml property

Получает и задает XML‑файл, определяющий интерфейс Ribbon.

```csharp
public string RibbonXml { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyRibbonXmlDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();

            // Пример XML‑файла ленты для настройки ленты
            string ribbonXml = 
                "<customUI xmlns=\"http://schemas.microsoft.com/office/2006/01/customui\">" +
                "  <ribbon>" +
                "    <tabs>" +
                "      <tab id=\"customTab\" label=\"My Tab\">" +
                "        <group id=\"customGroup\" label=\"My Group\">" +
                "          <button id=\"customButton\" label=\"My Button\" size=\"large\" />" +
                "        </group>" +
                "      </tab>" +
                "    </tabs>" +
                "  </ribbon>" +
                "</customUI>";

            // Установить свойство RibbonXml
            workbook.RibbonXml = ribbonXml;

            // Сохраните книгу
            workbook.Save("output.xlsm");

            // Проверить свойство RibbonXml
            Console.WriteLine("RibbonXml is set: " + (workbook.RibbonXml != null));
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


