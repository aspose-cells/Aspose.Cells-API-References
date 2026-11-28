---
title: "WorksheetCollection.RemoveAt"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Belirtilen bir adla öğeyi kaldırır"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Belirtilen adla öğeyi kaldırır.

```csharp
public void RemoveAt(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String | Kaldırılacak öğenin adı. |

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // Bazı çalışma sayfaları ekle
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");
            
            // Adlandırılmış bir aralık ekle (sabit)
            int nameIndex = wb.Worksheets.Names.Add("testname");
            wb.Worksheets.Names[nameIndex].RefersTo = "=[Book1.xlsx]Sheet1!$A1";
            
            // RemoveAt'i string parametresiyle göster
            Console.WriteLine($"Before removal - Worksheet count: {wb.Worksheets.Count}");
            wb.Worksheets.RemoveAt("Sheet1");
            Console.WriteLine($"After removal - Worksheet count: {wb.Worksheets.Count}");
            
            // Çalışma kitabını kaydedin
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int) {#removeat}

Belirtilen indeksteki öğeyi kaldırır.

```csharp
public void RemoveAt(int index)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Kaldırılacak öğenin indeks değeri. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // Bazı çalışma sayfaları ekle
            wb.Worksheets.Add("Sheet1");
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");

            // Orijinal çalışma sayfası sayısını göster
            Console.WriteLine($"Original worksheet count: {wb.Worksheets.Count}");

            // İndeks 1'deki çalışma sayfasını kaldır (ikinci çalışma sayfası)
            wb.Worksheets.RemoveAt(1);

            // Güncellenmiş çalışma sayfası sayısını göster
            Console.WriteLine($"After removal, worksheet count: {wb.Worksheets.Count}");

            // Çalışma kitabını kaydedin
            wb.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


