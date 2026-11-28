---
title: "WorksheetCollection.AddCopy"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Bir çalışma sayfasını koleksiyona ekler ve mevcut bir çalışma sayfasından verileri kopyalar"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/addcopy/
---
## AddCopy(string) {#addcopy_1}

Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar.

```csharp
public int AddCopy(string sheetName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | String | Kaynak çalışma sayfasının adı. |

### Dönüş Değeri

[`Worksheet`](../../worksheet/) object index.

### İstisnalar

| istisna | koşul |
| --- | --- |
| [CellsException](../../cellsexception/) | Geçersiz bir çalışma sayfası adı belirtir. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma kitabına "Original" adlı bir çalışma sayfası ekleyin
            Worksheet originalSheet = workbook.Worksheets.Add("Original");
            
            // Orijinal çalışma sayfasına bazı veriler ekleyin
            originalSheet.Cells["A1"].PutValue("This is the original sheet");
            
            // "Original" çalışma sayfasının bir kopyasını oluşturun
            int copiedIndex = workbook.Worksheets.AddCopy("Original");
            Worksheet copiedSheet = workbook.Worksheets[copiedIndex];
            copiedSheet.Name = "CopiedSheet";
            
            // Kopyalanan sayfayı, ayrı bir kopya olduğunu göstermek için değiştirin
            copiedSheet.Cells["A1"].PutValue("This is the copied sheet");
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetCopyDemo.xlsx");
            
            Console.WriteLine("Worksheet copied successfully. Output file: WorksheetCopyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(int) {#addcopy}

Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar.

```csharp
public int AddCopy(int sheetIndex)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | Int32 | Kaynak çalışma sayfasının indeksi. |

### Dönüş Değeri

[`Worksheet`](../../worksheet/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodAddCopyWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına erişin ve bazı veriler ekleyin
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Worksheet");
            
            // İlk çalışma sayfasının bir kopyasını ekleyin
            workbook.Worksheets.AddCopy(0);
            
            // Kopyanın oluşturulduğunu doğrulayın
            Worksheet copiedWorksheet = workbook.Worksheets[1];
            copiedWorksheet.Cells["A1"].PutValue("Copied Worksheet");
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddCopy(Worksheet[], string[]) {#addcopy_2}

Bir grup çalışma sayfasını kopyalar.

```csharp
public void AddCopy(Worksheet[] source, string[] destSheetNames)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| kaynak | Worksheet[] | Kaynak çalışma sayfaları. |
| destSheetNames | String[] | Kopyalanan sayfaların adları. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorksheetCollectionMethodAddCopyWithWorksheetStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bazı örnek çalışma sayfaları ekleyin
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Çalışma sayfalarına bazı veriler ekleyin
            workbook.Worksheets["Sheet2"].Cells["A1"].PutValue("Original Sheet1 Data");
            workbook.Worksheets["Sheet3"].Cells["A1"].PutValue("Original Sheet2 Data");

            // Kaynak çalışma sayfaları dizisini hazırlayın
            Worksheet[] sourceSheets = new Worksheet[]
            {
                workbook.Worksheets["Sheet2"],
                workbook.Worksheets["Sheet3"]
            };

            // Hedef sayfa adları dizisini hazırlayın
            string[] destSheetNames = new string[]
            {
                "CopyOfSheet2",
                "CopyOfSheet3"
            };

            try
            {
                // AddCopy metodunu (Worksheet[], String[]) parametreleriyle çağırın
                workbook.Worksheets.AddCopy(sourceSheets, destSheetNames);
                
                Console.WriteLine("AddCopy method executed successfully with parameters (Worksheet[], String[])");
                
                // Kopyaların oluşturulduğunu doğrulayın
                Console.WriteLine($"Total worksheets after copy: {workbook.Worksheets.Count}");
                foreach (Worksheet sheet in workbook.Worksheets)
                {
                    Console.WriteLine($"Worksheet name: {sheet.Name}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddCopy method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("WorksheetCollectionMethodAddCopyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


