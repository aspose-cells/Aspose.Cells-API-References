---
title: "Cells.ImportObjectArray"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir veri dizisini çalışma sayfasına aktarır"
type: docs
url: /tr/net/aspose.cells/cells/importobjectarray/
---
## ImportObjectArray(object[], int, int, bool) {#importobjectarray}

Bir çalışma sayfasına veri dizisi aktarır.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| objArray | Object[] | Veri dizisi. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| isVertical | Boolean | Verinin dikey mi yoksa yatay mı aktarılacağını belirtir. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veriyle bir nesne dizisi hazırlayın
            object[] dataArray = new object[] { "Product", "Price", "Stock", "Discontinued", 150.5, 75, false };

            try
            {
                // Nesne dizisini çalışma sayfasına B3 hücresinden (satır 2, sütun 1) başlayarak yatay şekilde aktarın
                worksheet.Cells.ImportObjectArray(dataArray, 2, 1, false);

                Console.WriteLine("Object array imported successfully to cells B3:F3");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Çıktıyı göstermek için çalışma kitabını kaydedin
            workbook.Save("CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportObjectArray(object[], int, int, bool, int) {#importobjectarray_1}

Bir çalışma sayfasına veri dizisi aktarır.

```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical, 
    int skip)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| objArray | Object[] | Veri dizisi. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| isVertical | Boolean | Verinin dikey mi yoksa yatay mı aktarılacağını belirtir. |
| atla | Int32 | Atlanan satır veya sütun sayısı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ImportObjectArray parametreleri için veriyi hazırlayın: (Object[], Int32, Int32, Boolean, Int32)
            object[] data = new object[]
            {
                "Name",
                "Age",
                "Date",
                "John Doe",
                30,
                new DateTime(2023, 10, 15),
                "Jane Smith",
                28,
                new DateTime(2023, 10, 16)
            };

            try
            {
                // ImportObjectArray'ı şu parametrelerle çağırın: (veri dizisi, başlangıç satırı 0, başlangıç sütunu 0, yatay aktarım, girişler arasında 1 sütun atla)
                worksheet.Cells.ImportObjectArray(data, 0, 0, false, 1);
                
                Console.WriteLine("Imported object array with parameters (Object[], 0, 0, false, 1) successfully.");
                
                // Etkiyi göster: Veriler A1, C1, E1, A2, C2, E2 vb. hücrelerine atlanmış sütunlarla yerleştirilecektir.
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportObjectArray: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


