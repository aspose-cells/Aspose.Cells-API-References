---
title: "Cell.Equals"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Bu nesnenin başka bir nesneyle aynı hücreye referans verip vermediğini kontrol eder"
type: docs
url: /tr/net/aspose.cells/cell/equals/
---
## Equals(object) {#equals_1}

Bu nesnenin aynı hücreye başka bir nesneyle referans verip vermediğini kontrol eder.

```csharp
public override bool Equals(object obj)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | Object | başka bir nesne |

### Dönüş Değeri

İki nesne aynı hücreye referans veriyorsa true.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Farklı konumlardan hücrelere eriş
            Cell cellA1 = worksheet.Cells["A1"];
            Cell anotherCellA1 = worksheet.Cells[0, 0]; // Same physical cell as A1
            Cell cellB1 = worksheet.Cells["B1"];

            // Farklı hücrelerde aynı değerleri ayarla
            cellA1.PutValue("Aspose.Cells");
            cellB1.PutValue("Aspose.Cells");

            try
            {
                // Aynı fiziksel hücre referanslarını karşılaştır
                bool sameCellComparison = cellA1.Equals(anotherCellA1);
                Console.WriteLine($"Same cell comparison: {sameCellComparison}"); // True

                // Aynı içeriğe sahip farklı hücreleri karşılaştır
                bool differentCellComparison = cellA1.Equals(cellB1);
                Console.WriteLine($"Different cell comparison: {differentCellComparison}"); // False

                // Hücreyi hücre olmayan bir nesneyle karşılaştır
                bool invalidTypeComparison = cellA1.Equals("Aspose.Cells");
                Console.WriteLine($"Invalid type comparison: {invalidTypeComparison}"); // False
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CellMethodEqualsWithObjectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Equals(Cell) {#equals}

Bu nesnenin aynı hücreye başka bir hücre nesnesiyle referans verip vermediğini kontrol eder.

```csharp
public bool Equals(Cell cell)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| hücre | Hücre | başka bir hücre nesnesi |

### Dönüş Değeri

İki hücre nesnesi aynı hücreye işaret ediyorsa doğru.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellMethodEqualsWithCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Farklı konumlarda (A1 ve B1) hücreler oluştur
            Cell cellA1 = worksheet.Cells[0, 0];
            Cell cellB1 = worksheet.Cells[0, 1];

            // Her iki hücreye aynı değerleri ayarla
            cellA1.Value = "Aspose.Cells Comparison";
            cellB1.Value = "Aspose.Cells Comparison";

            try
            {
                // cellA1'i cellB1 ile karşılaştır (farklı konumlar)
                bool equalsResult = cellA1.Equals(cellB1);
                Console.WriteLine($"Cell A1 equals Cell B1: {equalsResult}");

                // cellA1'i kendisiyle karşılaştır (aynı örnek)
                equalsResult = cellA1.Equals(cellA1);
                Console.WriteLine($"Cell A1 equals itself: {equalsResult}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Equals method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CellMethodEqualsWithCellDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


