---
title: "CellsDataTableFactory.GetInstance"
second_title: "Aspose.Cells için .NET API Referansı"
description: "CellsDataTableFactory yöntemi. Verilen tam sayı değerleri dizisinden ICellsDataTable oluşturur"
type: docs
url: /tr/net/aspose.cells/cellsdatatablefactory/getinstance/
---
## GetInstance(int[], string[]) {#getinstance_5}

Verilen tam sayı (integer) değer dizisinden ICellsDataTable oluşturur.

```csharp
public ICellsDataTable GetInstance(int[] vals, string[] columnNames)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| vals | Int32[] | tablo oluşturmak için tam sayı değerleri |
| columnNames | String[] | Tablonun sütun adları. Uzunluğu yalnızca 1 (tam sayı değerleriyle tabloyu dikey olarak oluştur) veya tam sayı değerlerinin uzunluğu (tam sayı değerleriyle tabloyu yatay olarak oluştur) olabilir |

### Dönüş Değeri

ICellsDataTable örneği

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32StringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yöntem parametreleri için verileri hazırla (Int32[], String[])
            int[] values = new int[] { 100, 200, 300, 400, 500 };
            string[] columnNames = new string[] { "Column1", "Column2", "Column3", "Column4", "Column5" };

            try
            {
                // Yansıma kullanarak CellsDataTableFactory örneği oluştur
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // (Int32[], String[]) parametreleriyle GetInstance'ı çağır
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Verileri çalışma sayfasına çıktı olarak ver
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Oluşturulan tablo hakkında bazı bilgileri göster
                Console.WriteLine("Method executed successfully with parameters (Int32[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Sütun adlarını yazdır
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32StringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[], bool) {#getinstance_4}

Verilen tam sayı (integer) değer dizisinden ICellsDataTable oluşturur.

```csharp
public ICellsDataTable GetInstance(int[] vals, bool vertial)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| vals | Int32[] | tablo oluşturmak için tam sayı değerleri |
| dikey | Boolean | tam sayı değerleriyle tabloyu dikey (true) ya da yatay (false) oluşturup oluşturmayacağını belirler |

### Dönüş Değeri

ICellsDataTable örneği

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithInt32ArrayBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yöntem parametreleri için verileri hazırla (Int32[], Boolean)
            int[] values = new int[] { 10, 20, 30, 40, 50 };
            bool vertical = true;

            try
            {
                // CellsDataTableFactory örneği oluştur
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // (Int32[], Boolean) parametreleriyle GetInstance'ı çağır
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Verileri çalışma sayfasına çıktı olarak ver
                int row = 0;
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully from Int32[] with vertical orientation");
                Console.WriteLine($"Total rows processed: {row}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("CellsDataTableFactoryGetInstanceWithInt32ArrayBooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], string[]) {#getinstance_2}

Verilen çift (double) değer dizisinden ICellsDataTable oluşturur.

```csharp
public ICellsDataTable GetInstance(double[] vals, string[] columnNames)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| vals | Double[] | tablo oluşturmak için çift değerler |
| columnNames | String[] | Tablonun sütun adları. Uzunluğu yalnızca 1 (çift değerlerle tabloyu dikey olarak oluştur) veya çift değerlerin uzunluğu (çift değerlerle tabloyu yatay olarak oluştur) olabilir. |

### Dönüş Değeri

ICellsDataTable örneği

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yöntem parametreleri için verileri hazırlayın (Double[], String[])
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            string[] columnNames = new string[] { "Price", "Cost", "Margin", "Tax", "Total" };

            try
            {
                // CellsDataTableFactory örneği oluştur
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // GetInstance'ı (Double[], String[]) parametreleriyle çağırın
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Verileri çalışma sayfasına çıktı olarak ver
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Oluşturulan tablo hakkında bilgileri göster
                Console.WriteLine("Method executed successfully with parameters (Double[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Sütun adlarını ve değerleri yazdır
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Değerleri yazdır
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int i = 0; i < dataTable.Columns.Length; i++)
                    {
                        Console.WriteLine($"{dataTable.Columns[i]}: {dataTable[i]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[], bool) {#getinstance_1}

Verilen çift (double) değer dizisinden ICellsDataTable oluşturur.

```csharp
public ICellsDataTable GetInstance(double[] vals, bool vertial)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| vals | Double[] | tablo oluşturmak için çift değerler |
| dikey | Boolean | çift değerlerle tabloyu vertiacally(true) veya horizontally(false) oluşturup oluşturmayacağını belirtir |

### Dönüş Değeri

ICellsDataTable örneği

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithDoubleBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yöntem parametreleri için verileri hazırlayın (Double[], Boolean)
            double[] values = new double[] { 10.5, 20.25, 30.75, 40.1, 50.9 };
            bool vertical = true;

            try
            {
                // CellsDataTableFactory örneği oluştur
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // GetInstance'ı (Double[], Boolean) ile çağırın
                ICellsDataTable dataTable = factory.GetInstance(values, vertical);

                // Verileri çalışma sayfasına çıktı olarak ver
                int row = 0;
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully with parameters (Double[], Boolean)");
                Console.WriteLine($"Total rows processed: {row}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("CellsDataTableFactoryGetInstanceWithDoubleBooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], string[]) {#getinstance_10}

Verilen nesne dizisinden ICellsDataTable oluşturur.

```csharp
public ICellsDataTable GetInstance(object[] vals, string[] columnNames)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| vals | Object[] | tablo oluşturmak için nesneler |
| columnNames | String[] | Tablonun sütun adları. Uzunluğu yalnızca 1 (nesnelerle tabloyu dikey olarak oluştur) veya nesnelerin uzunluğu (nesnelerle tabloyu yatay olarak oluştur) olabilir. |

### Dönüş Değeri

ICellsDataTable örneği

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yöntem parametreleri için verileri hazırlayın (Object[], String[])
            object[] values = new object[] { "John Doe", 35, 75000.50, DateTime.Now };
            string[] columnNames = new string[] { "Name", "Age", "Salary", "Hire Date" };

            try
            {
                // Yansıma kullanarak CellsDataTableFactory örneği oluştur
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // GetInstance metodunu (Object[], String[]) parametreleriyle çağırın
                ICellsDataTable dataTable = factory.GetInstance(values, columnNames);

                // Verileri, ImportDataTable yerine ImportData kullanarak çalışma sayfasına çıkartın
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                Console.WriteLine("Method executed successfully with parameters (Object[], String[])");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[][], bool, string[]) {#getinstance_11}

Verilen nesne dizisinden bir ICellsDataTable oluşturur.

```csharp
public ICellsDataTable GetInstance(object[][] vals, bool hasHeader, string[] columnNames)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| vals | Object[][] | tablo oluşturmak için nesneler |
| hasHeader | Boolean | İlk satırın başlık satırı olup olmadığını gösterir. |
| columnNames | String[] | Tablonun sütun adları. Uzunluğu yalnızca 1 (nesnelerle tabloyu dikey olarak oluştur) veya nesnelerin uzunluğu (nesnelerle tabloyu yatay olarak oluştur) olabilir. |

### Dönüş Değeri

ICellsDataTable örneği

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yöntem parametreleri için verileri hazırlayın (Object[][], Boolean, String[])
            object[][] data = new object[][]
            {
                new object[] { "ID", "Name", "Price" },
                new object[] { 1, "Laptop", 999.99 },
                new object[] { 2, "Phone", 699.99 },
                new object[] { 3, "Tablet", 399.99 }
            };

            bool hasHeader = true;
            string[] columnNames = new string[] { "ProductID", "ProductName", "ProductPrice" };

            try
            {
                // CellsDataTableFactory örneği oluştur
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // GetInstance'ı (Object[][], Boolean, String[]) ile çağırın
                ICellsDataTable dataTable = factory.GetInstance(data, hasHeader, columnNames);

                // Verileri çalışma sayfasına çıktı olarak ver
                int row = 0;
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully with parameters (Object[][], Boolean, String[])");
                Console.WriteLine($"Total rows processed: {row}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanStringDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[], bool) {#getinstance_9}

Verilen nesne dizisinden ICellsDataTable oluşturur.

```csharp
public ICellsDataTable GetInstance(object[] vals, bool vertial)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| vals | Object[] | tablo oluşturmak için nesneler |
| dikey | Boolean | nesnelerle tabloyu vertiacally(true) veya horizontally(false) oluşturup oluşturmayacağını belirtir |

### Dönüş Değeri

ICellsDataTable örneği

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsDataTableFactoryMethodGetInstanceWithObjectBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Yöntem parametreleri için verileri hazırlayın (Object[], Boolean)
            object[] data = new object[] { "Product", "Price", "Stock", "Available" };
            bool vertical = true;

            try
            {
                // Yansıma kullanarak CellsDataTableFactory örneği oluştur
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // GetInstance'ı (Object[], Boolean) parametreleriyle çağırın
                ICellsDataTable dataTable = factory.GetInstance(data, vertical);

                // Verileri çalışma sayfasına çıktı olarak ver
                dataTable.BeforeFirst();
                int row = 0;
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully with parameters (Object[], Boolean)");
                Console.WriteLine($"Data orientation: {(vertical ? "Vertical" : "Horizontal")}");
                Console.WriteLine($"Total items processed: {dataTable.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("CellsDataTableFactoryGetInstanceWithObjectBooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(int[]) {#getinstance_3}

```csharp
public ICellsDataTable GetInstance(int[] vals)
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(double[]) {#getinstance}

```csharp
public ICellsDataTable GetInstance(double[] vals)
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(object[]) {#getinstance_8}

```csharp
public ICellsDataTable GetInstance(object[] vals)
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection) {#getinstance_6}

Verilen koleksiyondan ICellsDataTable oluşturur.

```csharp
public ICellsDataTable GetInstance(ICollection collection)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| collection | ICollection | tablo oluşturmak için koleksiyon |

### Dönüş Değeri

ICellsDataTable örneği

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDataTableFactoryMethodGetInstanceWithICollectionDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ArrayList'i ICollection olarak hazırlayın
            ArrayList data = new ArrayList
            {
                new ArrayList { "Product", "Price", "Stock" },
                new ArrayList { "Keyboard", 49.99, 120 },
                new ArrayList { "Mouse", 29.99, 200 },
                new ArrayList { "Monitor", 199.99, 35 }
            };

            try
            {
                // CellsDataTableFactory örneği oluştur
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // GetInstance'ı ICollection parametresiyle çağırın
                ICellsDataTable dataTable = factory.GetInstance(data);

                // Verileri çalışma sayfasına çıktı olarak ver
                int row = 0;
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int col = 0; col < dataTable.Columns.Length; col++)
                    {
                        worksheet.Cells[row, col].PutValue(dataTable[col]);
                    }
                    row++;
                }

                Console.WriteLine("Data table created successfully from ICollection");
                Console.WriteLine($"Total rows processed: {row}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetInstance(ICollection, bool) {#getinstance_7}

Verilen koleksiyondan ICellsDataTable oluşturur.

```csharp
public ICellsDataTable GetInstance(ICollection collection, bool hasHeader)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| collection | ICollection | tablo oluşturmak için koleksiyon |
| hasHeader | Boolean | İlk satırın başlık olup olmadığını gösterir |

### Dönüş Değeri

ICellsDataTable örneği

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class CellsDataTableFactoryMethodGetInstanceWithICollectionBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Metod parametreleri için veri koleksiyonunu hazırla (ICollection, Boolean)
            ArrayList dataCollection = new ArrayList
            {
                new { Product = "Apple", Price = 2.5, Stock = 100 },
                new { Product = "Orange", Price = 1.8, Stock = 150 },
                new { Product = "Banana", Price = 0.9, Stock = 200 }
            };
            bool hasHeader = true;

            try
            {
                // CellsDataTableFactory örneği oluştur
                CellsDataTableFactory factory = (CellsDataTableFactory)Activator.CreateInstance(typeof(CellsDataTableFactory), nonPublic: true);
                
                // (ICollection, Boolean) parametreleriyle GetInstance'ı çağır
                ICellsDataTable dataTable = factory.GetInstance(dataCollection, hasHeader);

                // Verileri çalışma sayfasına çıktı olarak ver
                worksheet.Cells.ImportData(dataTable, 0, 0, new ImportTableOptions());

                // Oluşturulan tablo hakkında bilgileri göster
                Console.WriteLine("Method executed successfully with parameters (ICollection, Boolean)");
                Console.WriteLine($"Created table with {dataTable.Count} rows and {dataTable.Columns.Length} columns");
                
                // Sütun adlarını yazdır
                Console.WriteLine("Column Names:");
                foreach (string colName in dataTable.Columns)
                {
                    Console.WriteLine(colName);
                }

                // Değerleri yazdır
                dataTable.BeforeFirst();
                while (dataTable.Next())
                {
                    for (int i = 0; i < dataTable.Columns.Length; i++)
                    {
                        Console.WriteLine($"{dataTable.Columns[i]}: {dataTable[i]}");
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetInstance method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("CellsDataTableFactoryGetInstanceWithICollectionBooleanDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* interface [ICellsDataTable](../../icellsdatatable/)
* class [CellsDataTableFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


