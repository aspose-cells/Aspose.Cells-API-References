---
title: "Cell.SetStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cell yöntemi. Hücre stilini ayarlar"
type: docs
url: /tr/net/aspose.cells/cell/setstyle/
---
## SetStyle(Style) {#setstyle}

Hücre stilini ayarlar.

```csharp
public void SetStyle(Style style)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | Stil | Hücre stili. |

### Açıklamalar

Kenarlık ayarları değiştirildiğinde, ayarlanan hücrelerin kenarlığı da güncellenecektir.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Bir stil oluşturun ve özelliklerini ayarlayın
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.Yellow;

            // Stili B2 hücresine (sıfır tabanlı indekste 1,1) uygulayın
            cells[1, 1].SetStyle(style);

            // Çalışma kitabını kaydedin
            workbook.Save("SetStyleDemo.xlsx", SaveFormat.Xlsx);
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

## SetStyle(Style, bool) {#setstyle_2}

Stilin değiştirilmiş özelliğini hücreye uygular.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | Stil | Hücre stili. |
| explicitFlag | Boolean | Doğru, yalnızca açıkça ayarlanmış biçimlendirmeyi üzerine yazar. |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Stilleri doğrudan oluşturun
            Style style1 = workbook.CreateStyle();
            style1.Name = "MyStyle1";
            style1.Font.Name = "Arial";
            style1.Font.Size = 12;
            style1.Font.IsBold = true;
            
            Style style2 = workbook.CreateStyle();
            style2.Name = "MyStyle2";
            style2.Font.Name = "Times New Roman";
            style2.Font.Size = 14;
            style2.Font.Color = System.Drawing.Color.Red;
            
            // Stilleri hücrelere SetStyle yöntemiyle uygulayın
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("Styled Text 1");
            cell1.SetStyle(style1, true); // true to preserve existing style elements not defined in the new style
            
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Styled Text 2");
            cell2.SetStyle(style2, false); // false to overwrite all style elements
            
            // Çalışma kitabını kaydedin
            workbook.Save("SetStyleDemo.xlsx");
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

## SetStyle(Style, StyleFlag) {#setstyle_1}

Bayraklara göre hücre stilini uygula.

```csharp
public void SetStyle(Style style, StyleFlag flag)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| stil | Stil | Hücre stili. |
| bayrak | StyleFlag | Stil bayrağı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellMethodSetStyleWithStyleStyleFlagDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Bir stil oluşturun ve özelliklerini ayarlayın
            Style style = workbook.CreateStyle();
            style.Font.Color = Color.Red;
            style.Name = "CustomStyle";

            // Bir stil bayrağı oluşturun ve tüm biçimlendirmeyi uygulamak için ayarlayın
            StyleFlag flag = new StyleFlag();
            flag.All = true;

            // Hücreleri alın ve A1'e değer atayın
            Cells cells = sheet.Cells;
            Cell cell = cells["A1"];
            cell.PutValue("Sample Text");

            // Stili hücreye SetStyle kullanarak uygulayın
            cell.SetStyle(style, flag);

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [StyleFlag](../../styleflag/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


