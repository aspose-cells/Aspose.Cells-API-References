---
title: "CalculationData.GetParamValueInArrayMode"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationData yöntemi. Belirli bir indeksdeki parametrenin değerlerini alır. Parametre hesaplanması gereken bir ifade türü ise, dizi modunda hesaplanır"
type: docs
url: /tr/net/aspose.cells/calculationdata/getparamvalueinarraymode/
---
## CalculationData.GetParamValueInArrayMode method

Verilen indeksdeki parametrenin değer(ler)ini alır. Parametre hesaplanması gereken bir ifade ise, dizi modunda hesaplanır.

```csharp
public object[][] GetParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Parametrenin indeksi (0 tabanlı) |
| maxRowCount | Int32 | Döndürülen dizi için satır sayısı sınırı. Eğer sıfır veya negatif ya da gerçek satır sayısından büyükse, gerçek satır sayısı kullanılır. |
| maxColumnCount | Int32 | Döndürülen dizi için sütun sayısı sınırı. Eğer sıfır veya negatif ya da gerçek satır sayısından büyükse, gerçek sütun sayısı kullanılır. |

### Dönüş Değeri

Belirtilen parametreyle temsil edilen tüm öğeleri içeren bir dizi.

### Açıklamalar

Hesaplanması gereken bir ifade için, A:A+B:B örneğini alalım: Değer modunda, mevcut hücre temeline göre tek bir değere hesaplanır. Ancak dizi modunda, A1+B1, A2+B2, A3+B3, ... gibi tüm değerler hesaplanır ve döndürülen dizi oluşturmak için kullanılır. Böyle bir durumda, satır/sütun sayısı için bir sınır belirtmek (örneğin [`MaxDataRow`](../../cells/maxdatarow/) ve [`MaxDataColumn`](../../cells/maxdatacolumn/) değerlerine göre) daha iyidir; aksi takdirde döndürülen büyük dizi, gereksiz veri miktarıyla bellek maliyetini artırabilir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataMethodGetParamValueInArrayModeWithInt32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bağlam için örnek veri ekle
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Formula = "=SUM(A1:C3)";

            try
            {
                // Özel bir motorla hesaplama seçenekleri oluştur
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new ArrayModeCalculationEngine();
                workbook.CalculateFormula(options);

                Console.WriteLine("GetParamValueInArrayMode method called successfully");
                workbook.Save("GetParamValueInArrayModeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetParamValueInArrayMode: {ex.Message}");
            }
        }

        private class ArrayModeCalculationEngine : AbstractCalculationEngine
        {
            public override void Calculate(CalculationData data)
            {
                if (data.FunctionName == "SUM")
                {
                    // Gerçekçi parametrelerle GetParamValueInArrayMode yöntemini çağırın
                    object[][] paramArray = data.GetParamValueInArrayMode(0, 5, 3);

                    Console.WriteLine($"Parameter array dimensions: {paramArray.Length} rows");
                    if (paramArray.Length > 0)
                    {
                        Console.WriteLine($"First row has {paramArray[0].Length} columns");
                    }
                }
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


