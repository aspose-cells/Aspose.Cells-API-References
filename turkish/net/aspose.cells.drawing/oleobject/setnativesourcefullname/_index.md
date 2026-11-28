---
title: "OleObject.SetNativeSourceFullName"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject yöntemi. ole yerel kaynak tam dosya adını yol ile ayarlar"
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/setnativesourcefullname/
---
## OleObject.SetNativeSourceFullName method

Ole yerel kaynak tam dosya adını yol ile ayarlar.

```csharp
public void SetNativeSourceFullName(string sourceFullName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceFullName | String | ole yerel kaynak tam dosya adı |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class OleObjectMethodSetNativeSourceFullNameWithStringDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına bir OleObject ekle
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]); // Changed to empty byte array
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // SetNativeSourceFullName yöntemini bir dize parametresiyle çağırın
                oleObject.SetNativeSourceFullName(@"C:\temp\updated_test.xlsx");
                
                Console.WriteLine("SetNativeSourceFullName method executed successfully with parameter: C:\\temp\\updated_test.xlsx");
                
                // ObjectSourceFullName özelliğini kontrol ederek etkiyi gösterin
                Console.WriteLine($"OleObject's source is now: {oleObject.ObjectSourceFullName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetNativeSourceFullName method: {ex.Message}");
            }
            
            // Çalışma kitabını kaydedin
            workbook.Save("OleObjectMethodSetNativeSourceFullNameDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


