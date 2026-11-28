---
title: "Cells.GetCellsWithPlaceInCellPicture"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Cells yöntemi. Gömülü resim içeren tüm hücreleri alır"
type: docs
url: /tr/net/aspose.cells/cells/getcellswithplaceincellpicture/
---
## Cells.GetCellsWithPlaceInCellPicture method

Gömülü resim içeren tüm hücreleri alır.

```csharp
public IEnumerator GetCellsWithPlaceInCellPicture()
```

### Dönüş Değeri

Gömülü resim içeren tüm Cell nesnelerini yinelemek için Enumerator

### Açıklamalar

Bu çalışma sayfasında \"Place in Cell\" olarak ayarlanmış bir resim yoksa, null döndürülecektir.

### Örnekler

```csharp
using System;
using System.IO;
using System.Collections;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetCellsWithPlaceInCellPictureDemo
    {
        public static void Run()
        {
            // Bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Çalışma sayfasına bir resim ekle (bu, GetCellsWithPlaceInCellPicture tarafından sayılmayacaktır)
            workbook.Worksheets[0].Pictures.Add(0, 0, "sample.png");
            
            // B3 hücresine gömülü bir resim ekle (bu sayılacaktır)
            workbook.Worksheets[0].Cells["B3"].EmbeddedImage = File.ReadAllBytes("sample.png");
            
            // Yüzen resmi kaldır
            workbook.Worksheets[0].Pictures.RemoveAt(0);

            // Gömülü resim içeren hücreleri al
            Cells cells = workbook.Worksheets[0].Cells;
            int count = 0;
            
            IEnumerator enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                    Console.WriteLine($"Found image in cell {cell.Name}");
                }
            }
            
            Console.WriteLine($"Total cells with embedded images: {count}");
            
            // Kalıcı olmayı doğrulamak için kaydet ve yeniden yükle
            workbook.Save("output.xlsx");
            workbook = new Workbook("output.xlsx");
            
            // Yeniden yüklemeden sonra doğrula
            cells = workbook.Worksheets[0].Cells;
            count = 0;
            enumerator = cells.GetCellsWithPlaceInCellPicture();
            while (enumerator.MoveNext())
            {
                Cell cell = (Cell)enumerator.Current;
                byte[] imageData = cell.EmbeddedImage;
                if (imageData != null)
                {
                    count++;
                }
            }
            Console.WriteLine($"After reload - cells with embedded images: {count}");
        }
    }
}
```

### Ayrıca Bakınız

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


