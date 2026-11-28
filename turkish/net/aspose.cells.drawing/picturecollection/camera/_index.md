---
title: "PictureCollection.Camera"
second_title: "Aspose.Cells için .NET API Referansı"
description: "PictureCollection yöntemi. Aralığın fotoğrafını çeker"
type: docs
url: /tr/net/aspose.cells.drawing/picturecollection/camera/
---
## PictureCollection.Camera method

Aralığın fotoğrafını çeker.

```csharp
public int Camera(int row, int column, string range)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | Int32 | Bu resmin satır indeksi. |
| sütun | Int32 | Bu resmin sütun indeksi. |
| aralık | String | Fotoğraf çekilmesi gereken alan |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PictureCollectionMethodCameraWithInt32Int32StringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir aralık oluşturmak için bazı örnek veriler ekleyin
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";
            worksheet.Cells["A2"].Value = "Row 2";
            worksheet.Cells["B2"].Value = "Row 2 Col 2";

            try
            {
                // Çalışma sayfasından Pictures koleksiyonunu alın
                PictureCollection pictures = worksheet.Pictures;

                // Kamera resmini oluşturmak için Camera yöntemini çağırın
                // Parametreler: row (sol üst satır), column (sol üst sütun), range (kaynak aralık)
                int pictureIndex = pictures.Camera(5, 1, "A1:B2");

                Console.WriteLine($"Camera picture added successfully at index: {pictureIndex}");

                // Çalışma kitabını kaydedin
                workbook.Save("CameraDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Camera method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [PictureCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


