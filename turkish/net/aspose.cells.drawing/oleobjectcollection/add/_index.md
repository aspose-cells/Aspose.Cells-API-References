---
title: "OleObjectCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObjectCollection yöntemi. Bir OleObject'i koleksiyona ekler"
type: docs
url: /tr/net/aspose.cells.drawing/oleobjectcollection/add/
---
## Add(int, int, int, int, byte[]) {#add}

Koleksiyona bir OleObject ekler.

```csharp
public int Add(int topRow, int leftColumn, int height, int width, byte[] imageData)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| yükseklik | Int32 | oleObject'in yüksekliği, piksel biriminde. |
| genişlik | Int32 | oleObject'in genişliği, piksel biriminde. |
| imageData | Byte[] | ole nesnesinin görüntüsü bayt dizisi olarak. |

### Dönüş Değeri

[`OleObject`](../../oleobject/) object index.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // OLE nesne verisini hazırlayın (örnek Excel dosyası bayt dizisi olarak)
            byte[] oleData;
            try
            {
                string sampleFilePath = "sample.xlsx";
                oleData = File.ReadAllBytes(sampleFilePath);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error reading sample file: {ex.Message}");
                return;
            }

            try
            {
                // Add metodunu şu parametrelerle çağırın: (upperLeftRow, upperLeftColumn, height, width, imageData)
                int oleIndex = worksheet.OleObjects.Add(5, 2, 200, 300, oleData);

                Console.WriteLine($"OLE object added successfully at index: {oleIndex}");
                Console.WriteLine($"Position: Row 5, Column 2");
                Console.WriteLine($"Size: 200px height, 300px width");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("OleObjectAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## Add(int, int, int, int, byte[], string) {#add_1}

Koleksiyona bağlı bir OleObject ekler.

```csharp
public int Add(int topRow, int leftColumn, int height, int width, byte[] imageData, 
    string linkedFile)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| topRow | Int32 | Sol üst satır indeksi. |
| leftColumn | Int32 | Sol üst sütun indeksi. |
| yükseklik | Int32 | oleObject'in yüksekliği, piksel biriminde. |
| genişlik | Int32 | oleObject'in genişliği, piksel biriminde. |
| imageData | Byte[] | ole nesnesinin görüntüsü bayt dizisi olarak. |
| linkedFile | String |  |

### Dönüş Değeri

[`OleObject`](../../oleobject/) object index.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class OleObjectCollectionMethodAddWithInt32Int32Int32Int32ByteStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // OLE nesne verisini hazırlayın
            int upperLeftRow = 1;
            int upperLeftColumn = 1;
            int height = 200;
            int width = 200;
            byte[] imageData = File.ReadAllBytes("sample.ole");
            string linkedFile = "sample.xlsx";

            try
            {
                // Add metodunu belirli parametre tipleriyle çağırın
                int index = worksheet.OleObjects.Add(upperLeftRow, upperLeftColumn, height, width, imageData, linkedFile);
                
                Console.WriteLine($"OLE object added at index: {index}");
                Console.WriteLine($"Total OLE objects in worksheet: {worksheet.OleObjects.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("OleObjectAddDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObjectCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


