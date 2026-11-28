---
title: "Cell.GetStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Hücrenin stilini alır"
type: docs
url: /tr/net/aspose.cells/cell/getstyle/
---
## GetStyle() {#getstyle}

Hücre stilini al.

```csharp
public Style GetStyle()
```

### Dönüş Değeri

Stil nesnesi.

### Açıklamalar

Hücrenin stilini değiştirmek için, döndürülen stil nesnesini değiştirdikten sonra lütfen Cell.SetStyle() yöntemini çağırın. Bu yöntem, parametre için true değeriyle `GetStyle` ile aynıdır.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Hücreler için farklı dikey hizalamalar ayarlayın
            cells["A1"].PutValue("Bottom Alignment");
            cells["A1"].GetStyle().VerticalAlignment = TextAlignmentType.Bottom;

            cells["A2"].PutValue("Center Alignment");
            cells["A2"].GetStyle().VerticalAlignment = TextAlignmentType.Center;

            cells["A3"].PutValue("Distributed Alignment");
            cells["A3"].GetStyle().VerticalAlignment = TextAlignmentType.Distributed;

            cells["A4"].PutValue("Justify Alignment");
            cells["A4"].GetStyle().VerticalAlignment = TextAlignmentType.Justify;

            cells["A5"].PutValue("Top Alignment");
            cells["A5"].GetStyle().VerticalAlignment = TextAlignmentType.Top;

            // GetStyle() yöntemini göster
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("A2 Vertical Alignment: " + cells["A2"].GetStyle().VerticalAlignment);
            Console.WriteLine("A3 Vertical Alignment: " + cells["A3"].GetStyle().VerticalAlignment);
            Console.WriteLine("A4 Vertical Alignment: " + cells["A4"].GetStyle().VerticalAlignment);
            Console.WriteLine("A5 Vertical Alignment: " + cells["A5"].GetStyle().VerticalAlignment);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetStyle(bool) {#getstyle_1}

checkBorders true ise, diğer hücrelerin kenarlıklarının bu hücrenin stilini etkileyip etkilemeyeceğini kontrol et.

```csharp
public Style GetStyle(bool checkBorders)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| checkBorders | Boolean | Diğer hücrelerin kenarlıklarını kontrol edin |

### Dönüş Değeri

Stil nesnesi.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir hücreye erişin ve bazı örnek verileri ayarlayın
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue(123.456);

            // Satır/sütundan devralmadan hücrenin stilini al (false parametresi)
            Style style = cell.GetStyle(false);
            
            // Stili değiştir
            style.Custom = "0.000";
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.None;

            // Değiştirilen stili hücreye uygula
            cell.SetStyle(style);

            // Stil değişikliklerini doğrula
            Console.WriteLine("Number Format: " + cell.GetStyle(false).Custom);
            Console.WriteLine("Top Border Style: " + cell.GetStyle(false).Borders[BorderType.TopBorder].LineStyle);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


