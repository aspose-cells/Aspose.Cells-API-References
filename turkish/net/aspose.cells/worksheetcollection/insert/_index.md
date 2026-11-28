---
title: "WorksheetCollection.Insert"
second_title: "Aspose.Cells için .NET API Referansı"
description: "WorksheetCollection yöntemi. Bir çalışma sayfası ekle"
type: docs
url: /tr/net/aspose.cells/worksheetcollection/insert/
---
## Insert(int, SheetType) {#insert}

Bir çalışma sayfası ekle.

```csharp
public Worksheet Insert(int index, SheetType sheetType)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Çalışma sayfası indeksi |
| sheetType | SheetType | Çalışma sayfası türü. |

### Dönüş Değeri

Eklenen bir çalışma sayfasını döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Insert(1, SheetType.Worksheet);
            worksheet.Name = "InsertedSheet";
            workbook.Worksheets[0].Cells["A1"].Value = "Referencing inserted sheet:";
            workbook.Worksheets[0].Cells["A2"].Formula = "='InsertedSheet'!A1";
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Insert(int, SheetType, string) {#insert_1}

Bir çalışma sayfası ekle.

```csharp
public Worksheet Insert(int index, SheetType sheetType, string sheetName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| indeks | Int32 | Çalışma sayfası indeksi |
| sheetType | SheetType | Çalışma sayfası türü. |
| sheetName | String | Çalışma sayfası adı. |

### Dönüş Değeri

Eklenen bir çalışma sayfasını döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İndeks 0'da adı "InsertedSheet" olan yeni bir çalışma sayfası ekle
            workbook.Worksheets.Insert(0, SheetType.Worksheet, "InsertedSheet");
            
            // Eklenen çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Eklenen sayfanın A1 hücresine bazı veriler koy
            worksheet.Cells["A1"].PutValue("This sheet was inserted using Insert method");
            
            // Çalışma kitabını kaydedin
            workbook.Save("WorksheetInsertDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


