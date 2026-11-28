---
title: "Workbook.UpdateLinkedDataSource"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Bu workbook diğer veri kaynaklarına dış bağlantılar içeriyorsa Aspose.Cells, verilen kaynaklardan en son verileri almaya çalışacaktır."
type: docs
url: /tr/net/aspose.cells/workbook/updatelinkeddatasource/
---
## Workbook.UpdateLinkedDataSource method

Bu çalışma kitabı diğer veri kaynaklarına dış bağlantılar içeriyorsa, Aspose.Cells verilen kaynaklardan en son verileri almaya çalışacaktır.

```csharp
public void UpdateLinkedDataSource(Workbook[] externalWorkbooks)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| externalWorkbooks | Workbook[] | Bu workbook tarafından referans verilen dış bağlantıların verilerini güncellemek için kullanılacak Workbooks. Bu workbooks ile dış bağlantıların eşleşmesi [`FileName`](../filename/) ve [`DataSource`](../../externallink/datasource/) tarafından belirlenir. Bu yüzden her workbook için uygun değerde [`FileName`](../filename/) belirtildiğinden emin olun, böylece ilgili dış bağlantıya bağlanabilirler. |

### Açıklamalar

Bir workbook için ilgili dış bağlantı bulunamazsa, o workbook yok sayılacaktır. Bu yüzden daha sonra yeni bir dış bağlantı ile bir formül ayarladığınızda ve yok sayılan workbook'un ona bağlanmasını istediğinizde, bağlantı bu workbooks ile bu yöntemi tekrar çağırana kadar gerçekleştirilemez.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookMethodUpdateLinkedDataSourceWithWorkbookDemo
    {
        public static void Run()
        {
            // Dış referanslarla ana bir workbook oluşturun
            Workbook mainWorkbook = new Workbook();
            Worksheet mainSheet = mainWorkbook.Worksheets[0];
            mainSheet.Cells["A1"].Formula = "=[ExternalWorkbook.xlsx]Sheet1!A1";

            // Bağlanacak dış bir workbook oluşturun
            Workbook externalWorkbook = new Workbook();
            Worksheet externalSheet = externalWorkbook.Worksheets[0];
            externalSheet.Cells["A1"].Value = "Updated External Value";

            try
            {
                // Dış workbook dizisiyle UpdateLinkedDataSource yöntemini çağırın
                mainWorkbook.UpdateLinkedDataSource(new Workbook[] { externalWorkbook });

                // Referansı güncellemek için formülleri hesaplayın
                mainWorkbook.CalculateFormula();

                // Güncellenmiş değeri gösterin
                Console.WriteLine("Updated value in main workbook: " + mainSheet.Cells["A1"].Value);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing UpdateLinkedDataSource method: {ex.Message}");
            }

            // Sonucu kaydet
            mainWorkbook.Save("UpdateLinkedDataSourceDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


