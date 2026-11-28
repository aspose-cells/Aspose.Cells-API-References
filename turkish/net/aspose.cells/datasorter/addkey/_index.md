---
title: "DataSorter.AddKey"
second_title: "Aspose.Cells için .NET API Referansı"
description: "DataSorter yöntemi. Sıralanan sütun indeksini ve sıralama düzenini ekler"
type: docs
url: /tr/net/aspose.cells/datasorter/addkey/
---
## AddKey(int, SortOrder) {#addkey_1}

Sıralanmış sütun indeksini ve sıralama düzenini ekler.

```csharp
public void AddKey(int key, SortOrder order)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | Int32 | Sıralanmış sütun indeksi (mutlak konum, A sütunu 0, B 1, ...) |
| sıralama | SortOrder | Sıralama düzeni |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Sütun B (indeks 1) için artan sıralama anahtarı ekle
            workbook.DataSorter.AddKey(1, SortOrder.Ascending);
            
            // Veri aralığını sırala (A1:B4)
            workbook.DataSorter.Sort(worksheet.Cells, 0, 0, 3, 1);

            // Sıralanmış değerleri çıktıla
            Console.WriteLine("Sorted by Age (Ascending):");
            for (int i = 1; i <= 3; i++)
            {
                Console.WriteLine($"{worksheet.Cells[$"A{i+1}"].StringValue}: {worksheet.Cells[$"B{i+1}"].IntValue}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string) {#addkey_2}

Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama yönünü ekler.

```csharp
public void AddKey(int key, SortOrder order, string customList)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | Int32 | Sıralanmış sütun indeksi (mutlak konum, A sütunu 0, B 1, ...) |
| sıralama | SortOrder | Sıralama düzeni. |
| customList | String | Özel sıralama listesi. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DataSorterMethodAddKeyWithInt32SortOrderStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sıralanacak örnek veri
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("ddd");
            worksheet.Cells["A3"].PutValue("aaa");
            worksheet.Cells["A4"].PutValue("ccc");
            worksheet.Cells["A5"].PutValue("bbb");

            // Veri sıralayıcı oluştur ve özel sıralama anahtarını ekle
            DataSorter sorter = workbook.DataSorter;
            sorter.AddKey(0, SortOrder.Ascending, "aaa,ddd,ccc,bbb");
            sorter.HasHeaders = true;

            // Verileri sırala
            sorter.Sort(worksheet.Cells, CellArea.CreateCellArea("A1", "A5"));

            // Sonucu kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOnType, SortOrder, object) {#addkey}

Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama yönünü ekler.

```csharp
public void AddKey(int key, SortOnType type, SortOrder order, object customList)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | Int32 | Sıralanmış sütun indeksi (mutlak konum, A sütunu 0, B 1, ...) |
| type | SortOnType | Sıralanmış değer türü. |
| sıralama | SortOrder | Sıralama düzeni. |
| customList | Object | Özel sıralama listesi. |

### Açıklamalar

Tip SortOnType.CellColor veya SortOnType.FontColor ise, customList Color tipindedir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue(35);

            // Bir veri sıralayıcı oluştur
            DataSorter sorter = workbook.DataSorter;
            sorter.HasHeaders = true;

            try
            {
                // AddKey'i şu parametrelerle çağır: (Int32, SortOnType, SortOrder, Object)
                sorter.AddKey(
                    1,                          // Column index (B column)
                    SortOnType.Value,           // Sort on values (fixed from Values to Value)
                    SortOrder.Ascending,        // Sort order
                    null                        // Custom list (null for default)
                );

                // Sıralanacak aralığı tanımla
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 3;
                area.EndColumn = 1;

                // Verileri sırala
                sorter.Sort(worksheet.Cells, area);

                Console.WriteLine("Data sorted successfully using AddKey with parameters (Int32, SortOnType, SortOrder, Object)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddKey method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("DataSorterMethodAddKeyWithInt32SortOnTypeSortOrderObjectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SortOnType](../../sortontype/)
* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## AddKey(int, SortOrder, string[]) {#addkey_3}

Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama yönünü ekler.

```csharp
public void AddKey(int key, SortOrder order, string[] customList)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | Int32 | Sıralanmış sütun indeksi (mutlak konum, A sütunu 0, B 1, ...) |
| sıralama | SortOrder | Sıralama düzeni. |
| customList | String[] | Özel sıralama listesi. |

### Ayrıca Bakınız

* enum [SortOrder](../../sortorder/)
* class [DataSorter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


