---
title: "Cells.GroupColumns"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Sütunları gruplar"
type: docs
url: /tr/net/aspose.cells/cells/groupcolumns/
---
## GroupColumns(int, int) {#groupcolumns}

Sütunları gruplar.

```csharp
public void GroupColumns(int firstIndex, int lastIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | Int32 | Gruplanacak ilk sütun indeksi. |
| lastIndex | Int32 | Gruplanacak son sütun indeksi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Sütunları 0 ile 255 indeksleri arasında grupla
            cells.GroupColumns(0, 255);

            // Çalışma kitabını kaydedin
            string outputPath = "outputGroupColumns.xlsx";
            workbook.Save(outputPath);

            Console.WriteLine("Columns grouped successfully. File saved to: " + outputPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GroupColumns(int, int, bool) {#groupcolumns_1}

Sütunları gruplar.

```csharp
public void GroupColumns(int firstIndex, int lastIndex, bool isHidden)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstIndex | Int32 | Gruplanacak ilk sütun indeksi. |
| lastIndex | Int32 | Gruplanacak son sütun indeksi. |
| isHidden | Boolean | Gruplanan sütunların gizli olup olmadığını belirtir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGroupColumnsWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // 5 ile 7 arasındaki sütunları (3 sütun) grupla ve gizle
            cells.GroupColumns(5, 7, true);

            // Çalışma kitabını kaydedin
            workbook.Save("GroupColumnsOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


