---
title: "Cells.ImportCustomObjects"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Özel nesneleri içe aktarır"
type: docs
url: /tr/net/aspose.cells/cells/importcustomobjects/
---
## ImportCustomObjects(ICollection, string[], bool, int, int, int, bool, string, bool) {#importcustomobjects_1}

Özel nesneleri içe aktarır.

```csharp
public int ImportCustomObjects(ICollection list, string[] propertyNames, bool isPropertyNameShown, 
    int firstRow, int firstColumn, int rowNumber, bool insertRows, string dateFormatString, 
    bool convertStringToNumber)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| liste | ICollection | Özel nesne |
| propertyNames | String[] | Özellik adları. Null ise, nesnenin tüm özelliklerini içe aktaracağız. |
| isPropertyNameShown | Boolean | Özellik adının ilk satıra aktarılıp aktarılmayacağını gösterir. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| rowNumber | Int32 | İçe aktarılacak satır sayısı. |
| insertRows | Boolean | Veriye sığması için ekstra satırların eklenip eklenmeyeceğini gösterir. |
| dateFormatString | String | Hücreler için tarih biçim dizesi. |
| convertStringToNumber | Boolean | Bu yöntemin dizeyi sayıya dönüştürmeye çalışıp çalışmayacağını gösterir. |

### Dönüş Değeri

İthal edilen toplam satır sayısı.

### Açıklamalar

Özel nesneler aynı türde olmalıdır.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections.Generic;

    public class CellsMethodImportCustomObjectsWithICollectionStringBooleanInt3Demo
    {
        public class Product
        {
            public string Name { get; set; }
            public decimal Price { get; set; }
            public int Stock { get; set; }
            public DateTime Date { get; set; }
        }

        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            List<Product> products = new List<Product>
            {
                new Product { Name = "Apple", Price = 2.99m, Stock = 150, Date = new DateTime(2023, 12, 31) },
                new Product { Name = "Orange", Price = 1.99m, Stock = 200, Date = new DateTime(2024, 1, 15) }
            };

            string[] propertyNames = { "Name", "Price", "Stock", "Date" };

            try
            {
                int importedRows = worksheet.Cells.ImportCustomObjects(
                    products,
                    propertyNames,
                    true,
                    0,
                    0,
                    products.Count,
                    true,
                    "yyyy-MM-dd",
                    true
                );

                Console.WriteLine($"Successfully imported {importedRows} rows");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportCustomObjects: {ex.Message}");
            }

            workbook.Save("ImportCustomObjectsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportCustomObjects(ICollection, int, int, ImportTableOptions) {#importcustomobjects}

Özel nesneleri içe aktarır.

```csharp
public int ImportCustomObjects(ICollection list, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| liste | ICollection | Özel nesne |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| seçenekler | ImportTableOptions | İçe aktarma seçenekleri. |

### Dönüş Değeri

İthal edilen toplam satır sayısı.

### Açıklamalar

Özel nesneler aynı türde olmalıdır.

### Örnekler

```csharp
using System;
using System.Collections;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Customer
    {
        public int CustomerId { get; set; }
        public string Name { get; set; }
    }

    public class CellsMethodImportCustomObjectsWithICollectionInt32Int32ImportTabDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            List<Customer> customerList = new List<Customer>();

            for (int i = 0; i < 5; i++)
            {
                customerList.Add(new Customer
                {
                    CustomerId = i,
                    Name = "Customer" + i
                });
            }

            ImportTableOptions options = new ImportTableOptions
            {
                IsFieldNameShown = false,
                TotalRows = customerList.Count,
                InsertRows = true,
                DateFormat = "dd/mm/yyyy",
                ConvertNumericData = true,
                CheckMergedCells = true
            };

            wb.Worksheets[0].Cells.ImportCustomObjects((ICollection)customerList, 1, 0, options);
            wb.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


