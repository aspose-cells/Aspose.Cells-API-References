---
title: "Cells.ImportArrayList"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Cells. Импортирует ArrayList данных в лист"
type: docs
url: /ru/net/aspose.cells/cells/importarraylist/
---
## Cells.ImportArrayList method

Импортирует ArrayList данных в рабочий лист.

```csharp
public void ImportArrayList(ArrayList arrayList, int firstRow, int firstColumn, bool isVertical)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| arrayList | ArrayList | ArrayList данных. |
| firstRow | Int32 | Номер строки первой ячейки для импорта. |
| firstColumn | Int32 | Номер столбца первой ячейки для импорта. |
| isVertical | Boolean | Указывает импортировать данные вертикально или горизонтально. |

### Примеры

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportArrayListWithArrayListInt32Int32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            ArrayList data = new ArrayList();
            data.Add("Name");
            data.Add("Age");
            data.Add("City");
            
            cells.ImportArrayList(data, 0, 0, false);
            
            data.Clear();
            data.Add("John");
            data.Add(30);
            data.Add("New York");
            
            cells.ImportArrayList(data, 1, 0, false);
            
            workbook.Save("ImportArrayListDemo.xlsx");
        }
    }
}
```

### См. также

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


