---
title: "XmlMap.DataBinding"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlMap. Получает XmlDataBinding этой карты"
type: docs
url: /ru/net/aspose.cells/xmlmap/databinding/
---
## XmlMap.DataBinding property

Получает [`XmlDataBinding`](../../xmldatabinding/) этой карты.

```csharp
public XmlDataBinding DataBinding { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlMapPropertyDataBindingDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавить примерные XML‑карты
            string url1 = "https://example.com/data1.xml";
            string url2 = "https://example.com/data2.xml";
            
            // Добавить первую XML‑карту
            int mapIndex1 = workbook.Worksheets.XmlMaps.Add(url1);
            XmlMap map1 = workbook.Worksheets.XmlMaps[mapIndex1];
            
            // Добавить вторую XML‑карту
            int mapIndex2 = workbook.Worksheets.XmlMaps.Add(url2);
            XmlMap map2 = workbook.Worksheets.XmlMaps[mapIndex2];
            
            // Продемонстрировать использование свойства DataBinding
            Console.WriteLine("First XML Map:");
            Console.WriteLine("Name: " + map1.Name);
            Console.WriteLine("Root Element: " + map1.RootElementName);
            Console.WriteLine("Data Binding URL: " + map1.DataBinding.Url);
            
            Console.WriteLine("\nSecond XML Map:");
            Console.WriteLine("Name: " + map2.Name);
            Console.WriteLine("Root Element: " + map2.RootElementName);
            Console.WriteLine("Data Binding URL: " + map2.DataBinding.Url);
            
            // Сохраните книгу
            workbook.Save("XmlMapDataBindingDemo.xlsx");
        }
    }
}
```

### См. также

* class [XmlDataBinding](../../xmldatabinding/)
* class [XmlMap](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


