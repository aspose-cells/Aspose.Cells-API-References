---
title: "XmlMap.RootElementName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlMap. Получает имя корневого элемента"
type: docs
url: /ru/net/aspose.cells/xmlmap/rootelementname/
---
## XmlMap.RootElementName property

Получает имя корневого элемента.

```csharp
public string RootElementName { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyRootElementNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте примерные данные
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Создать XML‑карту
            string xml = "<root><item><Name>Item1</Name><Value>100</Value></item></root>";
            int mapIndex = workbook.Worksheets.XmlMaps.Add(xml);
            
            // Получить и отобразить имя корневого элемента
            string rootElementName = workbook.Worksheets.XmlMaps[mapIndex].RootElementName;
            Console.WriteLine("Root Element Name: " + rootElementName);
        }
    }
}
```

### См. также

* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


