---
title: "Cells.ImportDataGrid"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir DataGrid'i çalışma sayfasına aktarır"
type: docs
url: /tr/net/aspose.cells/cells/importdatagrid/
---
## ImportDataGrid(DataGrid, int, int, bool) {#importdatagrid}

Bir DataGrid'i çalışma sayfasına içe aktarır.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, bool insertRows)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataGrid | DataGrid | Aktarılacak DataGrid nesnesi. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| insertRows | Boolean | Veriye sığması için ekstra satırların eklenip eklenmeyeceğini gösterir. |

### Dönüş Değeri

Aktarılan toplam satır sayısı

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;
    using System.Data;

    public class CellsMethodImportDataGridWithDataGridInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // DataGrid verilerini taklit etmek için bir DataTable oluşturun
            DataTable dataTable = new DataTable();
            dataTable.Columns.Add("Name");
            dataTable.Columns.Add("Age");
            dataTable.Rows.Add("John", 30);
            dataTable.Rows.Add("Jane", 25);

            try
            {
                // API'de bulunan ImportDataView kullanarak verileri içe aktarın
                worksheet.Cells.ImportDataView(dataTable.DefaultView, 0, 0);

                Console.WriteLine("Data imported successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("ImportDataGridDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataGrid(DataGrid, int, int, int, int, bool) {#importdatagrid_1}

Bir DataGrid'i çalışma sayfasına içe aktarır.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataGrid | DataGrid | Aktarılacak DataGrid nesnesi. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| totalRows | Int32 | İçe aktarılacak satır sayısı. |
| totalColumns | Int32 | İçe aktarılacak sütun sayısı. |
| insertRows | Boolean | Veriye sığması için ekstra satırların eklenip eklenmeyeceğini gösterir. |

### Dönüş Değeri

Aktarılan toplam satır sayısı

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            try
            {
                // Bazı veri içeren örnek bir DataGrid oluşturun
                // DataGrid verilerini taklit etmek için basit bir dize dizisi kullanma
                string[,] gridData = new string[,]
                {
                    { "Name", "Age", "City" },
                    { "John", "30", "New York" },
                    { "Jane", "25", "Chicago" },
                    { "Bob", "35", "Los Angeles" }
                };

                // Verileri, satır 0, sütun 0'dan başlayarak çalışma sayfasına aktarın
                cells.ImportArray(gridData, 0, 0);

                // Çalışma kitabını kaydedin
                workbook.Save("ImportDataGridDemo.xlsx");
                Console.WriteLine("Data imported successfully to ImportDataGridDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportDataGrid(DataGrid, int, int, int, int, bool, bool) {#importdatagrid_2}

Bir DataGrid'i çalışma sayfasına içe aktarır.

```csharp
public int ImportDataGrid(DataGrid dataGrid, int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool insertRows, bool importStyle)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataGrid | DataGrid | Aktarılacak DataGrid nesnesi. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| totalRows | Int32 | İçe aktarılacak satır sayısı. |
| totalColumns | Int32 | İçe aktarılacak sütun sayısı. |
| insertRows | Boolean | Veriye sığması için ekstra satırların eklenip eklenmeyeceğini gösterir. |
| importStyle | Boolean | Hücre stilinin aktarılıp aktarılmayacağını gösterir. |

### Dönüş Değeri

Aktarılan toplam satır sayısı

### Örnekler

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataGridWithDataGridInt32Int32Int32Int32Bo257661Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Normalde bir DataGrid'den gelen örnek verileri oluşturun
            var sampleData = new List<object[]>
            {
                new object[] { "Name", "Age", "City" },
                new object[] { "John", 30, "New York" },
                new object[] { "Jane", 25, "Los Angeles" },
                new object[] { "Bob", 35, "Chicago" }
            };

            try
            {
                // DataGrid kullanamadığımız için verileri doğrudan hücrelere aktarın
                for (int row = 0; row < sampleData.Count; row++)
                {
                    for (int col = 0; col < sampleData[row].Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(sampleData[row][col]);
                    }
                }

                Console.WriteLine("Data imported successfully to worksheet.");

                // Çalışma kitabını kaydedin
                workbook.Save("ImportDataGridDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error importing data: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


