---
title: "Cells.GetDependentsInCalculation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Hesaplanan sonucu belirli bir hücreye bağlı olan tüm hücreleri alır"
type: docs
url: /tr/net/aspose.cells/cells/getdependentsincalculation/
---
## Cells.GetDependentsInCalculation method

Hesaplanan sonucu belirli hücreye bağlı olan tüm hücreleri alır.

```csharp
public IEnumerator GetDependentsInCalculation(int row, int column, bool recursive)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Belirli hücrenin satır indeksi |
| sütun | Int32 | Belirli hücrenin sütun indeksi. |
| recursive | Boolean | Belirli hücreye doğrudan başvurmayan, ancak o hücrenin diğer yapraklarına başvuran bağımlıları döndürür. |

### Dönüş Değeri

Tüm bağımlılıkları (Cell nesneleri) listelemek için Enumerator

### Açıklamalar

Bu yöntemi kullanmak için, çalışma kitabının [`EnableCalculationChain`](../../formulasettings/enablecalculationchain/) için true değerine ayarlandığından ve bu ayarla tamamen hesaplandığından emin olun. Bu hücreye formül referansı yoksa, null döndürülecektir. Daha fazla detay ve örnek için lütfen [`GetDependentsInCalculation`](../../cell/getdependentsincalculation/) adresine bakın.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsMethodGetDependentsInCalculationWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve formülleri hesaplayın
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Formül bağımlılıklarını ayarlayın:
            // C1 = 10 (kaynak değer)
            // B1 = C1*2
            // A1 = B1+5
            cells["C1"].PutValue(10);
            cells["B1"].Formula = "C1*2";
            cells["A1"].Formula = "B1+5";

            // Bağımlılıkları oluşturmak için formülleri hesaplayın
            workbook.CalculateFormula();

            try
            {
                // C1 hücresi (satır 0, sütun 2) için bağımlıları, özyinelemeli kontrolle alın
                IEnumerator dependents = cells.GetDependentsInCalculation(0, 2, true);

                Console.WriteLine("Dependents of cell C1:");
                while (dependents.MoveNext())
                {
                    if (dependents.Current is Cell dependentCell)
                    {
                        Console.WriteLine($"- {dependentCell.Name}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetDependentsInCalculation: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("GetDependentsInCalculationDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


