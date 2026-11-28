---
title: "CalculationData.Cell"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CalculationData özelliği. Fonksiyonun bulunduğu Cell nesnesini alır"
type: docs
url: /tr/net/aspose.cells/calculationdata/cell/
---
## CalculationData.Cell property

Fonksiyonun bulunduğu Cell nesnesini alır.

```csharp
public Cell Cell { get; }
```

### Açıklamalar

Bir formülü bir hücreye ayarlamadan, örneğin [`CalculateFormula`](../../worksheet/calculateformula/) ile hesaplandığında, formül A1 hücresine ayarlanmış gibi hesaplanır, bu yüzden hem [`CellRow`](../cellrow/) hem de [`CellColumn`](../cellcolumn/) 0 olur. Ancak, çalışma sayfasındaki A1 hücresi henüz oluşturulmamış olabilir. Bu tür durumlarda bu özellik null olacaktır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationDataPropertyCellDemo
    {
        public static void Run()
        {
            try
            {
                // Yeni bir çalışma kitabı oluştur
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Örneği anlamlı kılmak için bazı veriler ekleyin
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(20);
                worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

                // Özel bir motorla hesaplama seçenekleri oluştur
                CalculationOptions options = new CalculationOptions();
                options.CustomEngine = new CellDemoEngine();

                // Seçeneklerle formülleri hesaplayın.
                workbook.CalculateFormula(options);

                // Sonucu göster
                Console.WriteLine("A3 calculated value: " + worksheet.Cells["A3"].Value);

                // Sonucu kaydet
                workbook.Save("CellDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CellDemoEngine : AbstractCalculationEngine
    {
        public override void Calculate(CalculationData data)
        {
            if (data.FunctionName == "SUM")
            {
                // Salt okunur Cell özelliğine eriş
                Cell cell = data.Cell;
                Console.WriteLine($"Function is in cell: {cell.Name}");
                Console.WriteLine($"Cell value: {cell.StringValue}");
                Console.WriteLine($"Cell row: {cell.Row}, column: {cell.Column}");

                double sum = 0;
                for (int i = 0; i < data.ParamCount; i++)
                {
                    object arg = data.GetParamValue(i);
                    if (arg is double)
                    {
                        sum += (double)arg;
                    }
                }
                data.CalculatedValue = sum;
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [CalculationData](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


