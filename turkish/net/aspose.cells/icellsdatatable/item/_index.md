---
title: "ICellsDataTable.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ICellsDataTable özelliği. Belirtilen indeks tarafından tanımlanan sütunda depolanan verileri alır"
type: docs
url: /tr/net/aspose.cells/icellsdatatable/item/
---
## ICellsDataTable indexer (1 of 2)

Belirtilen indeks tarafından tanımlanan sütunda depolanan verileri alır.

```csharp
public object this[int columnIndex] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| columnIndex | Sütunun sıfır tabanlı indeksi. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo
    {
        public static void Run()
        {
            // Örnek veri ile özel ICellsDataTable oluşturun
            ICellsDataTable dataTable = new SampleDataTable();

            // İmleç konumunu sıfırla
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data using Item property:");
            while (dataTable.Next())
            {
                // Değerlere sütun indeksiyle erişin
                Console.WriteLine($"Product: {dataTable[0]}, Price: {dataTable[1]}, Stock: {dataTable[2]}");

                // Değerlere sütun adıyla erişin
                Console.WriteLine($"Product: {dataTable["Product"]}, Price: {dataTable["Price"]}, Stock: {dataTable["Stock"]}\n");
            }
        }
    }

    internal class SampleDataTable : ICellsDataTable
    {
        private readonly string[] columns = { "Product", "Price", "Stock" };
        private readonly object[][] data = 
        {
            new object[] { "Laptop", 999.99, 15 },
            new object[] { "Phone", 699.99, 25 },
            new object[] { "Tablet", 299.99, 50 }
        };
        private int currentRow = -1;

        public string[] Columns => columns;
        public int Count => data.Length;

        public object this[int columnIndex] => data[currentRow][columnIndex];
        public object this[string columnName] => data[currentRow][Array.IndexOf(columns, columnName)];

        public void BeforeFirst() => currentRow = -1;
        public bool Next() => ++currentRow < data.Length;
    }
}
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ICellsDataTable indexer (2 of 2)

Belirtilen sütun adıyla tanımlanan sütunda depolanan verileri alır.

```csharp
public object this[string columnName] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| columnName | Sütun adı. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ICellsDataTablePropertyItemDemo1
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek verileri hücrelere doldurun
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(499.99);

            // Veri aralığını açık dönüşümle ICellsDataTable'a dışa aktar
            ICellsDataTable dataTable = (ICellsDataTable)worksheet.Cells.ExportDataTable(0, 0, 3, 2);

            // İlk kayıttan önceki konuma taşı
            dataTable.BeforeFirst();

            Console.WriteLine("Reading data table values:");
            while (dataTable.Next())
            {
                // Sütun adlarını (indeksleyici) kullanarak Item özelliğine erişin
                string product = dataTable["Product"].ToString();
                double price = Convert.ToDouble(dataTable["Price"]);

                Console.WriteLine($"Item[Product]: {product}, Item[Price]: {price}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ItemPropertyDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


