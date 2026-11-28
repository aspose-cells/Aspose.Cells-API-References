---
title: "Cells.ExportDataTableAsString"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Cells koleksiyonundaki verileri bir DataTable nesnesine dışa aktarır"
type: docs
url: /tr/net/aspose.cells/cells/exportdatatableasstring/
---
## ExportDataTableAsString(int, int, int, int) {#exportdatatableasstring}

[`Cells`](../) koleksiyonundaki verileri bir DataTable nesnesine dışa aktarır.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Dışa aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | Dışa aktarılacak ilk hücrenin sütun numarası. |
| totalRows | Int32 | İçe aktarılacak satır sayısı. |
| totalColumns | Int32 | İçe aktarılacak sütun sayısı. |

### Dönüş Değeri

Dışa aktarılmış DataTable nesnesi.

### Açıklamalar

[`Cells`](../) koleksiyonundaki tüm veriler stringlere dönüştürülür.

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücrelere örnek veri ekle
            cells["A1"].PutValue("Column1");
            cells["B1"].PutValue("Column2");
            cells["A2"].PutValue("Value1");
            cells["B2"].PutValue("Value2");

            // Verileri DataTable'a string olarak dışa aktar
            DataTable dataTable = cells.ExportDataTableAsString(0, 0, 2, 2);

            // Dışa aktarılan verileri görüntüle
            Console.WriteLine("Exported DataTable:");
            foreach (DataColumn column in dataTable.Columns)
            {
                Console.Write(column.ColumnName + "\t");
            }
            Console.WriteLine();
            
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (var item in row.ItemArray)
                {
                    Console.Write(item.ToString() + "\t");
                }
                Console.WriteLine();
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

## ExportDataTableAsString(int, int, int, int, bool) {#exportdatatableasstring_1}

[`Cells`](../) koleksiyonundaki verileri bir DataTable nesnesine dışa aktarır.

```csharp
public DataTable ExportDataTableAsString(int firstRow, int firstColumn, int totalRows, 
    int totalColumns, bool exportColumnName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Dışa aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | Dışa aktarılacak ilk hücrenin sütun numarası. |
| totalRows | Int32 | İçe aktarılacak satır sayısı. |
| totalColumns | Int32 | İçe aktarılacak sütun sayısı. |
| exportColumnName | Boolean | İlk satırdaki verilerin DataTable'ın sütun adı olarak dışa aktarılıp aktarılmayacağını belirtir. |

### Dönüş Değeri

Dışa aktarılmış DataTable nesnesi.

### Açıklamalar

[`Cells`](../) koleksiyonundaki tüm veriler stringlere dönüştürülür.

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableAsStringWithInt32Int32Int32Int32BooleanDemo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Verileri DataTable'a dışa aktar
            int maxRow = worksheet.Cells.MaxDataRow + 1;
            int maxCol = worksheet.Cells.MaxDataColumn + 1;
            DataTable dataTable = worksheet.Cells.ExportDataTableAsString(0, 0, maxRow, maxCol, true);

            // Dışa aktarılan verileri görüntüle
            foreach (DataRow row in dataTable.Rows)
            {
                foreach (DataColumn col in dataTable.Columns)
                {
                    Console.Write(row[col] + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


