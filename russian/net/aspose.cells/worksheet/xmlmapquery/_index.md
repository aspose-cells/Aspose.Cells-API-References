---
title: "Worksheet.XmlMapQuery"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Worksheet. Запрос областей ячеек, сопоставленных/связанных с конкретным путем xml‑карты"
type: docs
url: /ru/net/aspose.cells/worksheet/xmlmapquery/
---
## Worksheet.XmlMapQuery method

Запрашивает области ячеек, сопоставленные/связанные с конкретным путём XML‑карты.

```csharp
[Obsolete("Use Worksheet.GetAreasOfXmlMapQuery() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList XmlMapQuery(string path, XmlMap xmlMap)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| путь | String | путь к элементу xml |
| xmlMap | XmlMap | Укажите xml‑карту, если хотите выполнить запрос конкретного пути внутри определённой карты |

### Возвращаемое значение

[`CellArea`](../../cellarea/) list that mapped/linked to the specific path of xml map, an empty list is returned if nothing is mapped/linked.

### Примечания

ПРИМЕЧАНИЕ: Этот метод теперь устарел. Вместо него, пожалуйста, используйте метод Worksheet.GetAreasOfXmlMapQuery(). Это свойство будет удалено через 12 месяцев, начиная с августа 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodXmlMapQueryWithStringXmlMapDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Добавить лист
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте пример XML‑карты
            string xml = @"<?xml version='1.0' encoding='UTF-8'?>
                <ns1:Root xmlns:ns1='http://example.com'>
                    <ns1:Data>
                        <ns1:Item>Value1</ns1:Item>
                    </ns1:Data>
                </ns1:Root>";
            
            // Импортируйте XML для создания карты
            workbook.ImportXml(xml, "Sheet1", 0, 0);
            
            // Получите XML‑карту
            XmlMap xmlMap = workbook.Worksheets.XmlMaps[0];
            
            // Запросите XML‑карту
            ArrayList cellAreas = worksheet.XmlMapQuery("/ns1:Root/ns1:Data/ns1:Item", xmlMap);
            
            // Вывести результаты
            if (cellAreas.Count > 0)
            {
                CellArea area = (CellArea)cellAreas[0];
                Console.WriteLine($"Found data at row {area.StartRow}, column {area.StartColumn}");
                Console.WriteLine($"Cell value: {worksheet.Cells[area.StartRow, area.StartColumn].StringValue}");
            }
        }
    }
}
```

### См. также

* class [XmlMap](../../xmlmap/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


