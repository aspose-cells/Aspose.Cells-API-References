---
title: "Cell.GetDependents"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Formülü doğrudan bu hücreye referans veren tüm hücreleri al."
type: docs
url: /tr/net/aspose.cells/cell/getdependents/
---
## Cell.GetDependents method

Formülü doğrudan bu hücreye referans veren tüm hücreleri al.

```csharp
public Cell[] GetDependents(bool isAll)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isAll | Boolean | Diğer çalışma sayfalarındaki formüllerin kontrol edilip edilmediğini gösterir. |

### Açıklamalar

Eğer bu hücreyi içeren bir referans bir hücrenin formülünde yer alıyorsa, o hücre bu hücrenin bağımlısı olarak kabul edilir; hesaplama sırasında referansın ya da bu hücrenin kullanılıp kullanılmadığına bakılmaksızın. Örneğin, "=IF(TRUE,A1,A2)" formülündeki A2 hücresi hesaplama sırasında kullanılmasa da, bu formül hâlâ A2'nin bağımlısı olarak kabul edilir. Bu hücreye bağlı olarak hesaplanan sonuçları olan formülleri elde etmek için lütfen [`GetDependentsInCalculation`](../getdependentsincalculation/) yöntemini kullanın. Bir hücrenin bağımlılarını izlerken, çalışma kitabındaki veya çalışma sayfasındaki tüm formüller analiz edilir ve kontrol edilir. Bu nedenle zaman tüketen bir işlemdir. Kullanıcı çok sayıda hücre için bağımlı izleme yapacaksa, bu yöntemi kullanmak performansı düşürür. Performans açısından, kullanıcı bunun yerine [`GetDependentsInCalculation`](../getdependentsincalculation/) yöntemini kullanmalıdır. Ya da kullanıcı önce [`GetPrecedents`](../getprecedents/) ile tüm hücrelerin öncül haritasını toplayıp, ardından öncül haritasına göre bağımlı haritasını oluşturabilir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetDependentsWithBooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // B1'i referans alan formülleri ayarla
            cells["A1"].Formula = "=B1+5";
            cells["A2"].Formula = "=B1*2";
            cells["A3"].Formula = "=SUM(B1:B3)";

            // Formülleri hesapla
            workbook.CalculateFormula();

            // B1'e bağımlı tüm hücreleri al (özyinelemeli)
            Cell[] dependents = cells["B1"].GetDependents(true);

            Console.WriteLine("Cells dependent on B1:");
            foreach (Cell cell in dependents)
            {
                Console.WriteLine(cell.Name + ": " + cell.Formula);
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


