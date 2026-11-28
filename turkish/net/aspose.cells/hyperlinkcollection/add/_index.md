---
title: "HyperlinkCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "HyperlinkCollection yöntemi. Belirtilen bir hücreye veya hücre aralığına bir köprü ekler"
type: docs
url: /tr/net/aspose.cells/hyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Belirtilen bir hücreye veya hücre aralığına bir hyperlink ekler.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | Int32 | Köprü aralığının ilk satırı. |
| firstColumn | Int32 | Köprü aralığının ilk sütunu. |
| totalRows | Int32 | Bu köprü aralığındaki satır sayısı. |
| totalColumns | Int32 | Bu köprü aralığındaki sütun sayısı. |
| address | String | Köprünün adresi. |

### Dönüş Değeri

[`Hyperlink`](../../hyperlink/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Satır/sütun koordinatları ve boyutları kullanarak köprü ekle
            worksheet.Hyperlinks.Add(0, 0, 1, 1, "http://www.aspose.com");
            worksheet.Hyperlinks.Add(1, 0, 1, 1, "c:\\book1.xls");
            
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_1}

Belirtilen bir hücreye veya hücre aralığına bir hyperlink ekler.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | String | Hücre adı. |
| totalRows | Int32 | Bu köprü aralığındaki satır sayısı. |
| totalColumns | Int32 | Bu köprü aralığındaki sütun sayısı. |
| address | String | Köprünün adresi. |

### Dönüş Değeri

[`Hyperlink`](../../hyperlink/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // A1 hücresine "www.aspose.com" adresli köprü ekle
            hyperlinks.Add("A1", 1, 1, "www.aspose.com");
            
            // Köprü adresini göster
            Console.WriteLine("Hyperlink Address: " + worksheet.Cells["A1"].StringValue);
            
            // Görüntüleme metnini değiştir
            worksheet.Cells["A1"].PutValue("Click Here");
            Console.WriteLine("Display Text: " + hyperlinks[0].TextToDisplay);
            
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, string, string) {#add_2}

Belirtilen bir hücreye veya hücre aralığına bir hyperlink ekler.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startCellName | String | Aralığın sol üst hücresi. |
| endCellName | String | Aralığın sağ alt hücresi. |
| address | String | Köprünün adresi. |
| textToDisplay | String | Belirtilen köprü için görüntülenecek metin. |
| screenTip | String | Belirtilen bağlantı için screenTip metni. |

### Dönüş Değeri

[`Hyperlink`](../../hyperlink/) object index.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Add metodunu (String, String, String, String, String) parametreleriyle gösterin.
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            workbook.Save("HyperlinkCollectionExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


