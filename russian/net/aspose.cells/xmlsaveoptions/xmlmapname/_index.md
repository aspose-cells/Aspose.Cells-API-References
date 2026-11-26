---
title: "XmlSaveOptions.XmlMapName"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство XmlSaveOptions. Указывает, экспортировать ли xml‑карту в файл"
type: docs
url: /ru/net/aspose.cells/xmlsaveoptions/xmlmapname/
---
## XmlSaveOptions.XmlMapName property

Указывает, экспортировать ли XML‑карту в файл.

```csharp
public string XmlMapName { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class XmlSaveOptionsPropertyXmlMapNameDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Заполните некоторые данные в листе
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);

            // Создать XML‑карту и добавить её в книгу
            int mapIndex = workbook.Worksheets.XmlMaps.Add("<Schema><Element><Product/><Price/></Element></Schema>");
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "ProductDataMap";

            // Создайте XmlSaveOptions и установите XmlMapName
            XmlSaveOptions saveOptions = new XmlSaveOptions();
            saveOptions.XmlMapName = "ProductDataMap";

            // Сохраните рабочую книгу с XML‑отображением
            workbook.Save("XmlWithMapping.xml", saveOptions);
        }
    }
}
```

### См. также

* class [XmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


