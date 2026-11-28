---
title: "Cells.ImportData"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Bir IDataReader nesnesinden veri ithal eder"
type: docs
url: /tr/net/aspose.cells/cells/importdata/
---
## ImportData(IDataReader, int, int) {#importdata_3}

IDataReader nesnesinden veri içe aktarır.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| okuyucu | IDataReader | Veri içeren IDataReader nesnesi. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |

### Dönüş Değeri

İthal edilen toplam satır sayısı.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Data;

    public class CellsMethodImportDataWithIDataReaderInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri tablosu oluştur
            DataTable dataTable = new DataTable("Employees");
            dataTable.Columns.Add("ID", typeof(int));
            dataTable.Columns.Add("Name", typeof(string));
            dataTable.Columns.Add("Department", typeof(string));
            
            dataTable.Rows.Add(1, "John Doe", "Engineering");
            dataTable.Rows.Add(2, "Jane Smith", "Marketing");
            dataTable.Rows.Add(3, "Mike Johnson", "Sales");

            try
            {
                // DataTable'dan IDataReader oluştur
                using (IDataReader dataReader = dataTable.CreateDataReader())
                {
                    // ImportData yöntemini A1 hücresinden (satır 0, sütun 0) başlayarak çağır
                    int importedRows = worksheet.Cells.ImportData(dataReader, 0, 0);
                    
                    Console.WriteLine($"Imported {importedRows} rows successfully.");
                    Console.WriteLine($"Data starts at: A1 (Row 0, Column 0)");
                }

                // Daha iyi görünürlük için sütunları otomatik sığdır
                worksheet.AutoFitColumns();
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ImportData method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("ImportDataWithIDataReader.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(IDataReader, int, int, ImportTableOptions) {#importdata_4}

IDataReader nesnesinden veri içe aktarır.

```csharp
public int ImportData(IDataReader reader, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| okuyucu | IDataReader | Veri içeren IDataReader nesnesi. |
| firstRow | Int32 | İçe aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | İçe aktarılacak ilk hücrenin sütun numarası. |
| seçenekler | ImportTableOptions | Tablo ithalatı seçenekleri. |

### Dönüş Değeri

İthal edilen toplam satır sayısı.

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithIDataReaderInt32Int32ImportTabDemo
    {
        public static void Run()
        {
            // Örnek bir DataTable oluştur
            DataTable dt = new DataTable("TestData");
            dt.Columns.Add("Column1", typeof(string));
            dt.Columns.Add("Column2", typeof(int));
            dt.Columns.Add("Column3", typeof(DateTime));
            
            // Örnek veri ekleyin.
            dt.Rows.Add("Data1", 100, DateTime.Now);
            dt.Rows.Add("Data2", 200, DateTime.Now.AddDays(1));
            dt.Rows.Add("Data3", 300, DateTime.Now.AddDays(2));

            // DataTableReader oluştur
            DataTableReader reader = dt.CreateDataReader();

            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // İthalat seçeneklerini ayarla
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;
            options.ConvertNumericData = true;
            options.DateFormat = "MM/dd/yyyy";

            // Veriyi satır 5, sütun 0'dan başlayarak ithal et
            int rowsImported = worksheet.Cells.ImportData(reader, 5, 0, options);

            // Çalışma kitabını kaydedin
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(ICellsDataTable, int, int, ImportTableOptions) {#importdata}

Özel veri tablosundan veri içe aktar.

```csharp
public int ImportData(ICellsDataTable table, int firstRow, int firstColumn, 
    ImportTableOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tablo | ICellsDataTable | Özel veri tablosu. |
| firstRow | Int32 | İlk satır indeksi. |
| firstColumn | Int32 | İlk sütun indeksi. |
| seçenekler | ImportTableOptions | İçe aktarma seçenekleri |

### Örnekler

```csharp
using System;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithICellsDataTableInt32Int32ImporDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            
            ArrayList dataLists = new ArrayList();
            dataLists.Add(new object[] { "Name", "Age", "Gender" });
            dataLists.Add(new object[] { "Alice", 30, "Female" });
            dataLists.Add(new object[] { "Bob", 25, "Male" });
            dataLists.Add(new object[] { "Charlie", 35, "Male" });

            ICellsDataTable dt = wb.CellsDataTableFactory.GetInstance(dataLists, true);
            
            wb.Worksheets[0].Cells.ImportData(dt, 0, 0, new ImportTableOptions());
            
            Console.WriteLine("Data imported to first worksheet:");
            Console.WriteLine(wb.Worksheets[0].Cells["A2"].StringValue);
            
            wb.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataTable, int, int, ImportTableOptions) {#importdata_1}

Özel veri tablosundan veri içe aktar.

```csharp
public int ImportData(DataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| tablo | DataTable | İçe aktarılacak DataTable nesnesi. |
| firstRow | Int32 | İlk satır indeksi. |
| firstColumn | Int32 | İlk sütun indeksi. |
| seçenekler | ImportTableOptions | İçe aktarma seçenekleri |

### Dönüş Değeri

İthal edilen toplam satır sayısı.

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithDataTableInt32Int32ImportTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Örnek DataTable oluştur
            DataTable dataTable = new DataTable("Products");
            dataTable.Columns.Add("Product_ID", typeof(int));
            dataTable.Columns.Add("Product_Name", typeof(string));
            dataTable.Columns.Add("Units_In_Stock", typeof(int));

            // Örnek veri ekleyin.
            DataRow row = dataTable.NewRow();
            row[0] = 1;
            row[1] = "Aniseed Syrup";
            row[2] = 15;
            dataTable.Rows.Add(row);

            row = dataTable.NewRow();
            row[0] = 2;
            row[1] = "Boston Crab Meat";
            row[2] = 123;
            dataTable.Rows.Add(row);

            // İthalat seçeneklerini ayarla
            ImportTableOptions importOptions = new ImportTableOptions();
            importOptions.IsFieldNameShown = true;

            // Verileri 5. satır, 5. sütundan başlayarak içe aktar
            cells.ImportData(dataTable, 5, 5, importOptions);

            // Çalışma kitabını kaydedin
            workbook.Save("ImportDataDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ImportData(DataView, int, int, ImportTableOptions) {#importdata_2}

Veri görünümünden veri içe aktar.

```csharp
public int ImportData(DataView dataView, int firstRow, int firstColumn, ImportTableOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dataView | DataView | İçe aktarılacak DataView nesnesi. |
| firstRow | Int32 | İlk satır indeksi. |
| firstColumn | Int32 | İlk sütun indeksi. |
| seçenekler | ImportTableOptions | İçe aktarma seçenekleri |

### Dönüş Değeri

İthal edilen toplam satır sayısı.

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodImportDataWithDataViewInt32Int32ImportTableODemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Örnek veri tablosu oluştur
            DataTable dataTable = new DataTable("TestTable");
            dataTable.Columns.Add("Column1", typeof(string));
            dataTable.Columns.Add("Column2", typeof(int));
            
            // Örnek veri ekleyin.
            dataTable.Rows.Add("Data1", 100);
            dataTable.Rows.Add("Data2", 200);
            dataTable.Rows.Add("Data3", 300);

            // ImportTableOptions oluşturun
            ImportTableOptions options = new ImportTableOptions();
            options.IsFieldNameShown = true;
            options.InsertRows = true;

            // Verileri DataView'den hücrelere, 0. satır, 0. sütundan başlayarak içe aktar
            cells.ImportData(dataTable.DefaultView, 0, 0, options);

            // Çalışma kitabını kaydedin
            workbook.Save("ImportDataOutput.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ImportTableOptions](../../importtableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


