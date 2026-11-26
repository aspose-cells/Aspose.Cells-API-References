---
title: "Cells.LinkToXmlMap"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Ссылка на XML‑карту"
type: docs
url: /ru/net/aspose.cells/cells/linktoxmlmap/
---
## Cells.LinkToXmlMap method

Ссылка на XML-карту.

```csharp
public void LinkToXmlMap(string mapName, int row, int column, string path)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| mapName | String | имя XML‑карты |
| строка | Int32 | строка целевой ячейки |
| column | Int32 | столбец целевой ячейки |
| путь | String | путь к элементу xml в xml‑карте |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodLinkToXmlMapWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook wb = new Workbook();
            
            // Добавить пример XML-карты
            int mapIndex = wb.Worksheets.XmlMaps.Add("<Transmittals><Issued_Document>Test</Issued_Document></Transmittals>");
            XmlMap xmlMap = wb.Worksheets.XmlMaps[mapIndex];
            xmlMap.Name = "Transmittals_Map";
            
            // Получить первый лист
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Связать ячейку с XML‑картой
            cells.LinkToXmlMap("Transmittals_Map", 0, 0, "/Transmittals/Issued_Document");
            
            // Сохраните книгу
            wb.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


