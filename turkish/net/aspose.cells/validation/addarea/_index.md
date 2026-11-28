---
title: "Validation.AddArea"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Validation yöntemi. Doğrulamayı alana uygular"
type: docs
url: /tr/net/aspose.cells/validation/addarea/
---
## AddArea(CellArea) {#addarea}

Doğrulamayı alana uygular.

```csharp
public void AddArea(CellArea cellArea)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | CellArea | Alan. |

### Açıklamalar

Kesişim ve kenar kontrolüyle `AddArea` kullanmaya eşdeğerdir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // Bir doğrulama oluştur
            ValidationCollection vc = sheet.Validations;
            Validation validation = vc[vc.Add(CellArea.CreateCellArea(0, 0, 0, 0))];
            validation.Type = ValidationType.List;
            validation.Formula1 = "=A1:A10";

            // Doğrulamaya daha fazla alan ekle
            for (int i = 1; i < 5; i++)
            {
                validation.AddArea(CellArea.CreateCellArea(i, 0, i, 0));
            }

            // Çalışma kitabını kaydedin
            wb.Save("ValidationMethodAddAreaWithCellAreaDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Validation with multiple areas created successfully.");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddArea(CellArea, bool, bool) {#addarea_1}

Doğrulamayı alana uygular.

```csharp
public void AddArea(CellArea cellArea, bool checkIntersection, bool checkEdge)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | CellArea | Alan. |
| checkIntersection | Boolean | Verilen alanın mevcut doğrulama alanlarıyla kesişimini kontrol edip etmeyeceği. Eğer bir doğrulama verilen alana (veya bir kısmına) uygulanmışsa, mevcut doğrulama önce verilen alandan kaldırılmalıdır. Aksi takdirde oluşturulan Validations bozulabilir. Kullanıcı, eklenen alanın herhangi bir mevcut alanla kesişmediğinden emin ise, performans açısından bu parametre false olarak ayarlanabilir. |
| checkEdge | Boolean | Bu doğrulamanın uygulanan alanlarının kenarının kontrol edilip edilmeyeceği. Validation'ın iç ayarları, uygulanan aralıkların sol üst (top-left) elemanına bağlıdır; bu nedenle verilen alan, uygulanan aralıkların yeni sol üst elemanı olacaksa, iç ayarlar değiştirilip yeniden oluşturulmalıdır, aksi takdirde beklenmeyen sonuçlar ortaya çıkabilir. Kullanıcı, eklenen alanın sol üst eleman olmadığından emin ise, performans açısından bu parametre false olarak ayarlanabilir. |

### Açıklamalar

Bu yöntemde, verilen alandaki tüm eski doğrulamaları kaldıracağız. Validation'ın uygulanan aralıklarının sol üst elemanı için, önce StartRow en küçük, ikinci olarak aynı en küçük StartRow değerine sahip alanlar arasında StartColumn en küçük olan seçilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodAddAreaWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur ve ilk çalışma sayfasını al
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Belirli bir alanda doğrulama oluştur
            Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(5, 3, 6, 3))];
            validation.Operator = OperatorType.GreaterThan;
            validation.Formula1 = "F3";

            // CellArea ve iki boolean parametre ile AddArea'yı göster
            validation.AddArea(CellArea.CreateCellArea(3, 3, 3, 4), false, true);
            Console.WriteLine("Area count after AddArea: " + validation.Areas.Length);
            Console.WriteLine("Formula1 after AddArea: " + validation.Formula1);

            // Eklenen alanı kaldır
            validation.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
            Console.WriteLine("Area count after RemoveArea: " + validation.Areas.Length);

            // Toplu işlemle birden fazla alan ekle
            CellArea[] areas = new CellArea[10];
            for (int i = 0; i < areas.Length; i++)
            {
                areas[i] = CellArea.CreateCellArea(6 + i, 3, 6 + i, 4);
            }
            validation.AddAreas(areas, true, true);
            Console.WriteLine("Area count after bulk AddAreas: " + validation.Areas.Length);

            // Çalışma kitabını kaydedin
            workbook.Save("ValidationMethodAddAreaDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


