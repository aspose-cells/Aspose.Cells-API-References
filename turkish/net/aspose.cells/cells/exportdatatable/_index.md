---
title: "Cells.ExportDataTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Cells koleksiyonundaki verileri bir DataTable nesnesine dışa aktarır"
type: docs
url: /tr/net/aspose.cells/cells/exportdatatable/
---
## ExportDataTable(int, int, int, int) {#exportdatatable}

[`Cells`](../) koleksiyonundaki verileri bir DataTable nesnesine dışa aktarır.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns)
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

Bu yöntemi bir veri bloğunu dışa aktarmak için kullanıyorsanız, bir sütundaki verilerin aynı veri tipinde olduğundan emin olun. Aksi takdirde, bunun yerine [`ExportDataTableAsString`](../exportdatatableasstring/) yöntemini kullanın.

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Örnek veri içeren bir çalışma kitabı oluşturun.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hücrelere örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["C1"].PutValue("City");
            
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells[i, 0].PutValue($"Person {i}");
                worksheet.Cells[i, 1].PutValue(20 + i);
                worksheet.Cells[i, 2].PutValue($"City {i}");
            }

            // Verileri DataTable'a dışa aktar (satır 0, sütun 0'dan başlayarak, 5 satır ve 3 sütun ile)
            DataTable dataTable = worksheet.Cells.ExportDataTable(0, 0, 5, 3);

            // Dışa aktarılan verileri görüntüle
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dataTable.Rows)
            {
                Console.WriteLine($"{row[0]}, {row[1]}, {row[2]}");
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

## ExportDataTable(int, int, int, int, bool) {#exportdatatable_2}

[`Cells`](../) koleksiyonundaki verileri bir DataTable nesnesine dışa aktarır.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    bool exportColumnName)
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

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32BooleanDemo
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

            // Verileri DataTable'a dışa aktar (ilk satır başlıkları içerir)
            DataTable dt = worksheet.Cells.ExportDataTable(0, 0, 3, 2, true);

            // Dışa aktarılan verileri görüntüle
            Console.WriteLine("Exported DataTable:");
            foreach (DataRow row in dt.Rows)
            {
                Console.WriteLine($"{row["Name"]}, {row["Age"]}");
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

## ExportDataTable(int, int, int, int, ExportTableOptions) {#exportdatatable_1}

[`Cells`](../) koleksiyonundaki verileri bir DataTable nesnesine dışa aktarır.

```csharp
public DataTable ExportDataTable(int firstRow, int firstColumn, int totalRows, int totalColumns, 
    ExportTableOptions options)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Dışa aktarılacak ilk hücrenin satır numarası. |
| firstColumn | Int32 | Dışa aktarılacak ilk hücrenin sütun numarası. |
| totalRows | Int32 | İçe aktarılacak satır sayısı. |
| totalColumns | Int32 | İçe aktarılacak sütun sayısı. |
| seçenekler | ExportTableOptions | Tüm dışa aktarma tablo seçenekleri |

### Dönüş Değeri

Dışa aktarılmış DataTable nesnesi.

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodExportDataTableWithInt32Int32Int32Int32ExportTablDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // A1 hücresi için değer ve biçim ayarla
            cells["A1"].PutValue(1.23356);
            Style style = cells["A1"].GetStyle();
            style.Custom = "0.00";
            cells["A1"].SetStyle(style);

            // Dışa aktarma seçeneklerini oluşturun
            ExportTableOptions etOpt = new ExportTableOptions();
            etOpt.ExportColumnName = false;
            etOpt.ExportAsString = true;

            // CellStyle biçim stratejisiyle dışa aktar
            etOpt.FormatStrategy = CellValueFormatStrategy.CellStyle;
            DataTable dt1 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("CellStyle format: " + dt1.Rows[0][0].ToString());

            // None biçim stratejisiyle dışa aktar
            etOpt.FormatStrategy = CellValueFormatStrategy.None;
            DataTable dt2 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("None format: " + dt2.Rows[0][0].ToString());

            // DisplayStyle biçim stratejisiyle dışa aktar
            etOpt.FormatStrategy = CellValueFormatStrategy.DisplayStyle;
            DataTable dt3 = cells.ExportDataTable(0, 0, 1, 1, etOpt);
            Console.WriteLine("DisplayStyle format: " + dt3.Rows[0][0].ToString());
        }
    }
}
```

### Ayrıca Bakınız

* class [ExportTableOptions](../../exporttableoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


