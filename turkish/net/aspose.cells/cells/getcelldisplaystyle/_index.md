---
title: "Cells.GetCellDisplayStyle"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen hücrenin görüntüleme stilini alır"
type: docs
url: /tr/net/aspose.cells/cells/getcelldisplaystyle/
---
## GetCellDisplayStyle(int, int) {#getcelldisplaystyle}

Verilen hücrenin görüntü stilini al.

```csharp
public Style GetCellDisplayStyle(int row, int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | belirtilen hücrenin satır indeksi |
| sütun | Int32 | belirtilen hücrenin sütunu |

### Dönüş Değeri

belirtilen hücrenin görüntüleme stili.

### Açıklamalar

Aynı şekilde [`GetDisplayStyle`](../../cell/getdisplaystyle/), ve aynı şekilde `GetCellDisplayStyle` için SideBorders kullanarak.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Gösterim için hücre stilini hazırlayın
            Cell cell = cells[0, 0];
            cell.PutValue("Style Demo");
            
            // Özel stil oluşturun
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            
            // Stili hücreye uygulayın
            cell.SetStyle(style);

            try
            {
                // Satır 0 ve sütun 0 ile GetCellDisplayStyle'ı çağırın
                Style displayStyle = cells.GetCellDisplayStyle(0, 0);

                // Görüntüleme stili özellikleri
                Console.WriteLine($"Bold: {displayStyle.Font.IsBold}");
                Console.WriteLine($"Background Color: {displayStyle.ForegroundColor}");

                // Görsel doğrulama için görüntüleme stilini başka bir hücreye uygulayın
                cells[2, 2].SetStyle(displayStyle);
                cells[2, 2].PutValue("Style Copied");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("CellsMethodGetCellDisplayStyleWithInt32Int32Demo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetCellDisplayStyle(int, int, BorderType) {#getcelldisplaystyle_1}

Verilen hücrenin görüntü stilini al.

```csharp
public Style GetCellDisplayStyle(int row, int column, BorderType adjacentBorders)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | belirtilen hücrenin satır indeksi |
| sütun | Int32 | belirtilen hücrenin sütunu |
| adjacentBorders | BorderType | Komşu hücrelerin kenarlarına göre hangi kenarların kontrol edilip ayarlanması gerektiğini gösterir. Aynı parametrenin açıklaması için lütfen [`GetDisplayStyle`](../../cell/getdisplaystyle/) bağlantısına bakın. |

### Dönüş Değeri

belirtilen hücrenin görüntüleme stili.

### Açıklamalar

Eğer hücre, koşullu biçimlendirme, liste nesneleri vb. gibi diğer ayarlardan da etkileniyorsa, görüntü stili [`GetCellStyle`](../getcellstyle/) yönteminden farklı olabilir. Ve bu ayarlar boş (var olmayan) hücrelere de uygulanabileceği için, bu yöntemi kullanmak bu boş hücrelerin örneklenmesini önleyebilir, böylece performans Cells üzerinden Cell örneği alıp ardından [`GetDisplayStyle`](../../cell/getdisplaystyle/) yöntemini çağırmaktan daha iyi olur.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetCellDisplayStyleWithInt32Int32BorderTypeDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // A1 hücresine erişin ve bir kenarlık stili ayarlayın
            Cell cell = worksheet.Cells["A1"];
            Style style = cell.GetStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            cell.SetStyle(style);

            try
            {
                // GetCellDisplayStyle yöntemini belirli parametrelerle (A1 için 0,0, TopBorder tipi) çağırın
                Style displayStyle = worksheet.Cells.GetCellDisplayStyle(0, 0, BorderType.TopBorder);

                // Alınan stilin kenarlık rengimizle eşleşip eşleşmediğini kontrol edin
                if (displayStyle.Borders[BorderType.TopBorder].Color == System.Drawing.Color.Red)
                {
                    Console.WriteLine("Top border display style retrieved successfully - Color: Red");
                }

                // Başka bir hücreyi değiştirerek stil uygulamasını gösterin
                Cell targetCell = worksheet.Cells["B1"];
                targetCell.SetStyle(displayStyle);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetCellDisplayStyle method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("GetCellDisplayStyleWithBorderTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Style](../../style/)
* enum [BorderType](../../bordertype/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


