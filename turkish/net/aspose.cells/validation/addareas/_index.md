---
title: "Validation.AddAreas"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Doğrulama yöntemi. Verilen alanlara doğrulamayı uygular."
type: docs
url: /tr/net/aspose.cells/validation/addareas/
---
## Validation.AddAreas method

Doğrulamayı verilen alanlara uygular.

```csharp
public void AddAreas(CellArea[] areas, bool checkIntersection, bool checkEdge)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| alanlar | CellArea[] | Alanlar. |
| checkIntersection | Boolean | Verilen alanın mevcut doğrulama alanlarıyla kesişimini kontrol edip etmeyeceği. Eğer bir doğrulama verilen alana (veya bir kısmına) uygulanmışsa, mevcut doğrulama önce verilen alandan kaldırılmalıdır. Aksi takdirde oluşturulan Validations'da bozulma meydana gelebilir. Kullanıcı, eklenen tüm alanların herhangi bir mevcut alanla kesişmediğinden emin ise, performans düşüncesiyle bu parametre false olarak ayarlanabilir. |
| checkEdge | Boolean | Bu doğrulamanın uygulanan alanlarının kenarının kontrol edilip edilmemesi. Doğrulamanın iç ayarları, uygulanan aralıkların sol‑üst noktasına bağlıdır; bu nedenle verilen alanlardan biri yeni sol‑üst nokta olursa, iç ayarlar değiştirilip yeniden oluşturulmalıdır, aksi takdirde beklenmeyen sonuçlar ortaya çıkabilir. Kullanıcı, eklenen alanların hiç birinin sol‑üst nokta olmadığından emin ise, performans düşüncesiyle bu parametre false olarak ayarlanabilir. |

### Açıklamalar

Bu yöntemde, verilen alandaki tüm eski doğrulamaları kaldıracağız. Validation'ın uygulanan aralıklarının sol üst elemanı için, önce StartRow en küçük, ikinci olarak aynı en küçük StartRow değerine sahip alanlar arasında StartColumn en küçük olan seçilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ValidationMethodAddAreasWithCellAreaBooleanBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int validationIndex = worksheet.Validations.Add();
            Validation validation = worksheet.Validations[validationIndex];
            validation.Type = ValidationType.List;
            validation.AlertStyle = ValidationAlertType.Stop;
            validation.Operator = OperatorType.None;
            validation.Formula1 = "1,2,3";
            validation.InCellDropDown = true;

            CellArea[] areas = new CellArea[2];
            areas[0] = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 1 };
            areas[1] = new CellArea { StartRow = 2, StartColumn = 2, EndRow = 3, EndColumn = 3 };

            try
            {
                validation.AddAreas(areas, true, false);
                Console.WriteLine("Added validation areas with checkIntersection=true, checkEdge=false");

                foreach (CellArea area in validation.Areas)
                {
                    Console.WriteLine($"Validation area: R{area.StartRow + 1}C{area.StartColumn + 1}:R{area.EndRow + 1}C{area.EndColumn + 1}");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding validation areas: {ex.Message}");
            }

            workbook.Save("ValidationAddAreasDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


