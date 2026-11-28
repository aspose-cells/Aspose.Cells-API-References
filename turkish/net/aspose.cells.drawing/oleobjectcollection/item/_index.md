---
title: "OleObjectCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObjectCollection özelliği. Belirtilen indeksteki OleObject öğesini alır"
type: docs
url: /tr/net/aspose.cells.drawing/oleobjectcollection/item/
---
## OleObjectCollection indexer

Belirtilen indeksteki [`OleObject`](../../oleobject/) öğesini alır.

```csharp
public OleObject this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | Öğenin sıfır tabanlı indeksi. |

### Dönüş Değeri

Belirtilen indeksteki öğe.

### Örnekler

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class OleObjectCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Örnek resim verisi ekle
            byte[] binaryImg = File.ReadAllBytes("image1.png");
            
            // İlk çalışma sayfasına OLE nesnesi ekle
            int idxOle = workbook.Worksheets[0].OleObjects.Add(0, 0, 60, 60, binaryImg);
            
            // OLE nesnesine Item özelliği kullanarak eriş
            OleObject objOle = workbook.Worksheets[0].OleObjects[idxOle];
            
            // Gömülü nesne özelliklerini ayarla
            byte[] binaryXlsx = File.ReadAllBytes("example.xlsx");
            objOle.SetEmbeddedObject(false, binaryXlsx, "SampleFile.xlsx", true, "Excel.Sheet", false);
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsx");
            
            // Kaydedilen dosyayı doğrula
            Workbook savedWorkbook = new Workbook("output.xlsx");
            Console.WriteLine("OLE Object Source: " + savedWorkbook.Worksheets[0].OleObjects[0].ObjectSourceFullName);
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../../oleobject/)
* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


