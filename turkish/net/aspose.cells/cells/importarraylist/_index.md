---
title: "Cells.ImportArrayList"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir veri arraylist'ini çalışma sayfasına aktarır"
type: docs
url: /tr/net/aspose.cells/cells/importarraylist/
---
## Cells.ImportArrayList method

Bir çalışma sayfasına veri arraylist'ini içe aktarır.

```csharp
public void ImportArrayList(ArrayList arrayList, int firstRow, int firstColumn, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arrayList | ArrayList | Veri arraylist'i. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| isVertical | Boolean | Verinin dikey mi yoksa yatay mı aktarılacağını belirtir. |

### Örnekler

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

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


