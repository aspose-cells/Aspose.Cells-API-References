---
title: "ListObject.PutCellFormula"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ListObject yöntemi. Formülü tablo içindeki hücreye yerleştirin"
type: docs
url: /tr/net/aspose.cells.tables/listobject/putcellformula/
---
## PutCellFormula(int, int, string) {#putcellformula}

Formülü tablodaki hücreye koy.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | Int32 | Tablodaki satır ofseti. |
| columnOffset | Int32 | Tablodaki sütun ofseti. |
| formül | String | Hücrenin formülü. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Bir tablo oluşturmak için örnek veri ekle
            sheet.Cells["A1"].PutValue("ID");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["C1"].PutValue("Formula");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["B3"].PutValue(20);

            // Bir liste nesnesi (tablo) oluştur
            int index = sheet.ListObjects.Add("A1", "C3", true);
            ListObject table = sheet.ListObjects[index];

            // Yeni bir satır ekleyin ve değerleri/formülü ayarlayın
            table.PutCellValue(4, 0, 3); // Row 4, Column 0 (ID)
            table.PutCellValue(4, 1, 30); // Row 4, Column 1 (Value)
            table.PutCellFormula(4, 2, "=B3*2"); // Row 4, Column 2 (Formula)

            // Çalışma kitabını kaydedin
            wb.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## PutCellFormula(int, int, string, bool) {#putcellformula_1}

Formülü tablodaki hücreye koy.

```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula, bool isTotalsRowFormula)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | Int32 | Tablodaki satır ofseti. |
| columnOffset | Int32 | Tablodaki sütun ofseti. |
| formül | String | Hücrenin formülü. |
| isTotalsRowFormula | Boolean |  |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodPutCellFormulaWithInt32Int32StringBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bir liste nesnesi oluşturmak için örnek veri ekleyin.
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            
            // Liste nesnesi oluştur
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];
            
            // PutCellFormula'ı göster
            listObject.PutCellFormula(3, 0, "=SUM(A2:A3)", true);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


