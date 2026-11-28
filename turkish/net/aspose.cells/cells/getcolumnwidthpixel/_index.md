---
title: "Cells.GetColumnWidthPixel"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Belirtilen sütunun normal görünümde piksel birimindeki genişliğini alır"
type: docs
url: /tr/net/aspose.cells/cells/getcolumnwidthpixel/
---
## GetColumnWidthPixel(int) {#getcolumnwidthpixel}

Normal görünümde belirtilen sütunun genişliğini piksel biriminde alır.

```csharp
public int GetColumnWidthPixel(int column)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi |

### Dönüş Değeri

Normal görünümde sütunun genişliği.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetColumnWidthPixelWithInt32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Sütun genişliğini karakter cinsinden ayarlayın (piksellere dönüştürülecek)
            worksheet.Cells.SetColumnWidth(1, 25);
            
            // Sütun genişliğini piksel olarak alın
            int widthInPixels = worksheet.Cells.GetColumnWidthPixel(1);
            
            // Sonucu çıktı olarak ver
            Console.WriteLine("Column width in pixels: " + widthInPixels);
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetColumnWidthPixel(int, bool) {#getcolumnwidthpixel_1}

Normal görünümde belirtilen sütunun genişliğini piksel biriminde alır.

```csharp
[Obsolete("Use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int GetColumnWidthPixel(int column, bool original)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | Int32 | Sütun indeksi |
| orijinal | Boolean | Sütun gizli olduğunda bile orijinal genişliğin döndürülüp döndürülmeyeceğini gösterir |

### Dönüş Değeri

Normal görünümde sütunun genişliği.

### Açıklamalar

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine lütfen Cells.GetColumnWidth(int ,bool , CellsUnitType ) yöntemini kullanın. Bu yöntem, Nisan 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetColumnWidthPixelWithInt32BooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasına erişin
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Standart sütun genişliğini 80 piksele ayarlayın
            worksheet.Cells.StandardWidthPixels = 80;

            // 2. sütun (üçüncü sütun) için belirli sütun genişliğini 120 piksele ayarlayın
            worksheet.Cells.SetColumnWidthPixel(2, 120);

            try
            {
                // Kullanıcı değişiklikleriyle mevcut genişliği alın (orijinal: false)
                int currentWidth = worksheet.Cells.GetColumnWidthPixel(2, false);
                Console.WriteLine($"Column 2 current width: {currentWidth} pixels");

                // Değişiklik olmadan orijinal genişliği alın (orijinal: true)
                int originalWidth = worksheet.Cells.GetColumnWidthPixel(2, true);
                Console.WriteLine($"Column 2 original width: {originalWidth} pixels");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetColumnWidthPixel: {ex.Message}");
            }

            // Sütun genişliği kalıcılığını göstermek için çalışma kitabını kaydedin
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


