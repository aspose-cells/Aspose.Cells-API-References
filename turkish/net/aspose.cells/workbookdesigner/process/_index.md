---
title: "WorkbookDesigner.Process"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorkbookDesigner yöntemi. Akıllı işaretçileri işler ve veri kaynağı değerlerini doldurur"
type: docs
url: /tr/net/aspose.cells/workbookdesigner/process/
---
## Process(Range, bool) {#process_1}

Akıllı işaretçileri işler ve veri kaynağı değerlerini doldurur.

```csharp
[Obsolete("Use Range smart markers instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Process(Range range, bool isPreserved)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| aralık | Aralık | İşlenecek aralık |
| isPreserved | Boolean | True, tanımlanamayan akıllı işaretçi korunuyorsa. |

### Açıklamalar

NOTE: Bu sınıf artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen Aralık akıllı işaretçilerini kullanın. Bu özellik, Temmuz 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithRangeBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = wb.Worksheets[0];
            
            // Hücrelerde örnek veri oluştur
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("&=$Name");
            sheet.Cells["B2"].PutValue("&=$Value");
            
            // Çalışma kitabı tasarımcısı oluştur
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = wb;
            
            // JSON veri kaynağı oluştur
            string jsonData = "{'Name':'Test Product','Value':100.50}";
            designer.SetJsonDataSource("Data", jsonData);
            
            // Akıllı işaretçilerle belirli aralığı işle
            Aspose.Cells.Range range = sheet.Cells.CreateRange("A2:B2");
            range.Name = "_CellsSmartMarkers";
            
            // Aralığı işle (true = sadece bu aralığı işle)
            designer.Process(range, true);
            
            // Sonucu kaydet
            wb.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Range](../../range/)
* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process() {#process}

Akıllı işaretçileri işler ve veri kaynağı değerlerini doldurur.

```csharp
public void Process()
```

### Örnekler

```csharp
using System;
using System.Collections;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessDemo
    {
        public static void Run()
        {
            // Şablon dosyasından bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");
            WorkbookDesigner designer = new WorkbookDesigner(workbook);

            // Veri kaynağını hazırla
            ArrayList persons = new ArrayList();
            
            Person person1 = new Person("John Doe", 30);
            person1.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person1);

            Person person2 = new Person("Jane Smith", 28);
            person2.FOTO = File.ReadAllBytes("1.jpg");
            persons.Add(person2);

            // Veri kaynağını ayarlayın ve işleyin
            designer.SetDataSource("Datos", persons);
            designer.Process();

            // Sonucu kaydet
            workbook.Save("output.xlsx");
        }
    }

    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }
        public byte[] FOTO { get; set; }

        public Person(string name, int age)
        {
            Name = name;
            Age = age;
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(bool) {#process_2}

Akıllı işaretçileri işler ve veri kaynağı değerlerini doldurur.

```csharp
public void Process(bool isPreserved)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| isPreserved | Boolean | True, tanımlanamayan akıllı işaretçi korunuyorsa. |

### Örnekler

```csharp
using System;
using System.Collections.Generic;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithBooleanDemo
    {
        public static void Run()
        {
            // Çalışma kitabını başlat ve şablonu yükle
            Workbook workbook = new Workbook("example.xlsx");
            
            // JSON'dan yüklemek yerine doğrudan örnek veri oluştur
            ABC_1_Data data = new ABC_1_Data
            {
                Directors = new List<Director>
                {
                    new Director { DRFNAME2 = "DRFNAME2" }
                }
            };

            // Akıllı işaretçileri ayarlayın
            workbook.Worksheets[0].Cells.CreateRange("A13:K19").Name = "_CellsSmartMarkers";

            // Veri kaynaklarını hazırla
            List<ABC_1_Data> listData = new List<ABC_1_Data> { data };

            // Çalışma kitabı tasarımcısını işle
            WorkbookDesigner designer = new WorkbookDesigner
            {
                Workbook = workbook,
                LineByLine = false
            };
            
            designer.SetDataSource("RootData", listData);
            designer.SetDataSource("Directors", data.Directors);
            
            // Boolean parametresiyle işle
            designer.Process(true);
            
            // Sonucu kaydedin
            workbook.Save("output.xlsx");
        }
    }

    // Örnek veri sınıfları
    public class ABC_1_Data
    {
        public List<Director> Directors { get; set; }
    }

    public class Director
    {
        public string DRFNAME2 { get; set; }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Process(int, bool) {#process_3}

Akıllı işaretçileri işler ve veri kaynağı değerlerini doldurur.

```csharp
public void Process(int sheetIndex, bool isPreserved)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | Int32 | Çalışma sayfası indeksi. |
| isPreserved | Boolean | True, tanımlanamayan akıllı işaretçi korunuyorsa. |

### Açıklamalar

Bu yöntem çalışma sayfası seviyesinde çalışır.

### Örnekler

```csharp
using System;
using System.Data;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookDesignerMethodProcessWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Kaynak dosyadan bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsx");
            
            // Çalışma sayfasındaki verileri DataTable'a dışa aktar
            Worksheet worksheet = workbook.Worksheets["Data"];
            DataTable dataTable = worksheet.Cells.ExportDataTable(
                0, 0, 
                worksheet.Cells.MaxDataRow, 
                worksheet.Cells.MaxDataColumn + 1, 
                new ExportTableOptions { 
                    CheckMixedValueType = true, 
                    ExportColumnName = true 
                });
            dataTable.TableName = "Table";

            // Çalışma kitabı tasarımcısını oluştur ve veri kaynağını ayarla
            WorkbookDesigner designer = new WorkbookDesigner();
            designer.Workbook = workbook;
            designer.SetDataSource(dataTable);

            // Tasarımcıyı parametrelerle (Int32, Boolean) işleyin
            designer.Process(0, true);

            // Sonucu kaydet
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [WorkbookDesigner](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


