---
title: "Cells.Find"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Girdi nesnesini içeren hücreyi bulur"
type: docs
url: /tr/net/aspose.cells/cells/find/
---
## Find(object, Cell) {#find}

Girdi nesnesini içeren hücreyi bulur.

```csharp
public Cell Find(object what, Cell previousCell)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ne | Object | Aranacak nesne. Tür int,double,DateTime,string,bool olmalıdır. |
| previousCell | Hücre | Aynı nesneye sahip önceki hücre. Aramaya baştan başlıyorsanız bu parametre null olarak ayarlanabilir. |

### Dönüş Değeri

Hücre nesnesi.

### Açıklamalar

Hiç hücre bulunamazsa null (Nothing) döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Örnek veri ekleyin
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B4"].PutValue(1.2);

            // "Orange" içeren hücreyi bulun
            Cell searchCell = null;
            Cell foundCell = worksheet.Cells.Find("Orange", searchCell);

            if (foundCell != null)
            {
                Console.WriteLine("Found 'Orange' at: " + foundCell.Name);
                
                // Bulunan hücreye bir stil oluştur ve uygula
                Style style = workbook.CreateStyle();
                style.Font.Color = System.Drawing.Color.Red;
                style.Font.IsBold = true;
                foundCell.SetStyle(style);
            }

            // Çalışma kitabını kaydedin
            workbook.Save("FindMethodDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Find(object, Cell, FindOptions) {#find_1}

Girdi nesnesini içeren hücreyi bulur.

```csharp
public Cell Find(object what, Cell previousCell, FindOptions findOptions)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ne | Object | Aranacak nesne. Tür int,double,DateTime,string,bool olmalıdır. |
| previousCell | Hücre | Aynı nesneye sahip önceki hücre. Aramaya baştan başlıyorsanız bu parametre null olarak ayarlanabilir. |
| findOptions | FindOptions | Bulma seçenekleri |

### Dönüş Değeri

Hücre nesnesi.

### Açıklamalar

Hiç hücre bulunamazsa null (Nothing) döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodFindWithObjectCellFindOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Örnek veriyi ayarla
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["A2"].PutValue("def");
            worksheet.Cells["A3"].PutValue("abc ");
            
            // Bulma seçenekleri oluştur
            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // Değeri "abc " olan hücreyi bulun
            Cell foundCell = worksheet.Cells.Find("abc ", null, options);
            
            Console.WriteLine("Found cell: " + (foundCell != null ? foundCell.Name : "null"));
        }
    }
}
```

### Ayrıca Bakınız

* class [Cell](../../cell/)
* class [FindOptions](../../findoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


