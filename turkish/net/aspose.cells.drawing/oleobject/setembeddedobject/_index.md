---
title: "OleObject.SetEmbeddedObject"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject yöntemi. Gömülü nesne verilerini ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/setembeddedobject/
---
## SetEmbeddedObject(bool, byte[], string, bool, string) {#setembeddedobject}

Gömülü nesne verisini ayarlar.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| linkToFile | Boolean | Nesnenin dosyaya bağlanıp bağlanmadığını gösterir. True ise, objectData parametresi yok sayılır. |
| objectData | Byte[] | Gömülü nesne verileri. |
| sourceFileName | String | Dosya adı. |
| displayAsIcon | Boolean | Nesnenin bir simge olarak gösterilip gösterilmeyeceğini belirtir. True ise, orijinal görüntü verisi simgeyle kaplanır. |
| label | String | Simge etiketi. Yalnızca displayAsIcon true olduğunda çalışır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir OleObject ekle
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // SetEmbeddedObject için parametreleri hazırla
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.xlsx");
                string sourceFileName = "sample.xlsx";
                bool displayAsIcon = false;
                string label = "Excel Document";

                // Belirtilen parametrelerle SetEmbeddedObject'i çağır
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String)");
                
                // Etkiyi göstermek için bazı özellikleri görüntüle
                Console.WriteLine($"OleObject label: {oleObject.Label}");
                Console.WriteLine($"Display as icon: {oleObject.DisplayAsIcon}");
                Console.WriteLine($"Is linked to file: {oleObject.IsLink}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetEmbeddedObject(bool, byte[], string, bool, string, bool) {#setembeddedobject_1}

Gömülü nesne verisini ayarlar.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label, bool updateIcon)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| linkToFile | Boolean | Nesnenin dosyaya bağlanıp bağlanmadığını gösterir. True ise, objectData parametresi yok sayılır. |
| objectData | Byte[] | Gömülü nesne verileri. |
| sourceFileName | String | Dosya adı. |
| displayAsIcon | Boolean | Nesnenin bir simge olarak gösterilip gösterilmeyeceğini belirtir. True ise, orijinal görüntü verisi simgeyle kaplanır. |
| label | String | Simge etiketi. Yalnızca displayAsIcon true olduğunda çalışır. |
| updateIcon | Boolean | Simgenin otomatik olarak güncellenip güncellenmeyeceğini belirtir. |

### Açıklamalar

Aspose tüm dosya simgelerini güncelleyebildiği için, *updateIcon* false olarak ayarlandığında doğru simgeyi eklemek daha iyidir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir OleObject ekle
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // SetEmbeddedObject için parametreleri hazırla
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.docx");
                string sourceFileName = "sample.docx";
                bool displayAsIcon = true;
                string label = "Word Document";
                bool updateIcon = true;

                // Belirtilen parametrelerle SetEmbeddedObject'i çağır
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label, updateIcon);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


