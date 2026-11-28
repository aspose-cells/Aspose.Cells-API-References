---
title: "Cell.GetLeafs"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Bu hücreye doğrudan referans veren ve hücre değiştirildiğinde güncellenmesi gereken tüm hücreleri al"
type: docs
url: /tr/net/aspose.cells/cell/getleafs/
---
## GetLeafs() {#getleafs}

Bu hücreye doğrudan referans veren ve hücre değiştirildiğinde güncellenmesi gereken tüm hücreleri al.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs()
```

### Dönüş Değeri

Tüm bağımlıları (Cell) yinelemek için Enumerator

### Açıklamalar

NOT: Bu sınıf artık eski. Bunun yerine, hesaplama zincirindeki tüm bağımlıları almak için lütfen Cell.GetDependentsInCalculation(bool) metodunu kullanın. Bu özellik Mayıs 2022'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağımlılıklar oluşturmak için bazı veri ve formüller ekle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Bağımlıları olan hücreyi al
                Cell cell = worksheet.Cells["B1"];

                // Bu hücreye doğrudan referans veren tüm hücreleri almak için GetLeafs'i çağır
                IEnumerator leafs = cell.GetLeafs();

                Console.WriteLine("Cells that directly reference B1:");
                while (leafs.MoveNext())
                {
                    Cell leafCell = leafs.Current as Cell;
                    if (leafCell != null)
                    {
                        Console.WriteLine($"Cell: {leafCell.Name}, Formula: {leafCell.Formula}");
                    }
                }

                // Çalışma kitabını kaydedin
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetLeafs(bool) {#getleafs_1}

Bu hücre değiştirildiğinde güncellenecek tüm hücreleri al.

```csharp
[Obsolete("Use GetDependentsInCalculation(bool) instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IEnumerator GetLeafs(bool recursive)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| recursive | Boolean | Doğrudan bu hücreye referans vermeyen ancak bu hücrenin diğer yapraklarına referans veren yaprakları döndürür mü |

### Dönüş Değeri

Tüm bağımlıları (Cell) yinelemek için Enumerator

### Açıklamalar

NOT: Bu sınıf artık eski. Bunun yerine, hesaplama zincirindeki tüm bağımlıları almak için lütfen Cell.GetDependentsInCalculation(bool) metodunu kullanın. Bu özellik Mayıs 2022'den itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellMethodGetLeafsWithBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağımlılıklar oluşturmak için formüllü bazı veri ekle
            worksheet.Cells["A1"].Value = 10;
            worksheet.Cells["A2"].Value = 20;
            worksheet.Cells["B1"].Formula = "=A1+A2";
            worksheet.Cells["C1"].Formula = "=B1*2";

            try
            {
                // Bağımlıları olan hücreyi al
                Cell cell = worksheet.Cells["A1"];

                // GetLeafs'i özyinelemeli parametre true olarak ayarlayarak çağır
                IEnumerator leafs = cell.GetLeafs(true);

                // Sonuçları görüntüleyin
                Console.WriteLine("Leaf cells found:");
                while (leafs.MoveNext())
                {
                    Cell leaf = (Cell)leafs.Current;
                    Console.WriteLine($"Cell: {leaf.Name}, Value: {leaf.Value}");
                }

                // Çalışma kitabını kaydedin
                workbook.Save("GetLeafsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetLeafs: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


