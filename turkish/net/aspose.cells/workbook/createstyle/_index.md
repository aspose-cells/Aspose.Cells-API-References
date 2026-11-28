---
title: "Workbook.CreateStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Yeni bir stil oluşturur"
type: docs
url: /tr/net/aspose.cells/workbook/createstyle/
---
## CreateStyle() {#createstyle}

Yeni bir stil oluşturur.

```csharp
public Style CreateStyle()
```

### Dönüş Değeri

Bir stil nesnesi döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // CreateStyle yöntemi kullanarak yeni bir stil oluştur
            Style newStyle = workbook.CreateStyle();
            
            // Stil özelliklerini ayarla
            newStyle.Font.Name = "Arial";
            newStyle.Font.Size = 12;
            newStyle.Font.IsBold = true;
            newStyle.ForegroundColor = System.Drawing.Color.LightBlue;
            newStyle.Pattern = BackgroundType.Solid;
            newStyle.IsTextWrapped = true;
            
            // Stil bayrağı oluştur ve bayrakları ayarla
            StyleFlag flag = new StyleFlag();
            flag.FontName = true;
            flag.FontSize = true;
            flag.FontBold = true;
            flag.CellShading = true;
            flag.WrapText = true;
            
            // Stili A1 hücresine uygula
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("This text has a custom style with wrapping");
            worksheet.Cells.ApplyStyle(newStyle, flag);
            
            // Sütunu otomatik sığdır
            worksheet.AutoFitColumn(0);
            
            // Çalışma kitabını kaydedin
            workbook.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CreateStyle(bool) {#createstyle_1}

Yeni bir stil oluşturur.

```csharp
public Style CreateStyle(bool cloneDefaultStyle)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cloneDefaultStyle | Boolean | Varsayılan stili kopyalayıp kopyalamadığını gösterir |

### Dönüş Değeri

Bir stil nesnesi döndürür.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodCreateStyleWithBooleanDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook wb = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Yeni bir stil oluştur (false = varsayılan stilden devralma)
            Style style = wb.CreateStyle(false);
            style.Font.Color = System.Drawing.Color.Blue;
            style.Font.IsBold = true;
            
            // Stili bir hücreye uygula
            Cell cell = cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Styled Text");
            
            // Çalışma kitabını kaydedin
            wb.Save("CreateStyleDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


