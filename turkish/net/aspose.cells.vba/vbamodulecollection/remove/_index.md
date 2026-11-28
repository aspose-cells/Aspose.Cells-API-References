---
title: "VbaModuleCollection.Remove"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaModuleCollection yöntemi. Bir çalışma sayfası için modülü kaldırır"
type: docs
url: /tr/net/aspose.cells.vba/vbamodulecollection/remove/
---
## Remove(Worksheet) {#remove}

Bir çalışma sayfası için modülü kaldırır.

```csharp
public void Remove(Worksheet sheet)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfa | Çalışma Sayfası | Çalışma sayfası |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Vba;
    using System;

    public class VbaModuleCollectionMethodRemoveWithWorksheetDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasına bir VBA modülü ekleyin
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // VBA modül koleksiyonunu alın
            VbaModuleCollection modules = workbook.VbaProject.Modules;
            
            try
            {
                // Çalışma sayfası parametresiyle Remove yöntemini çağırın
                modules.Remove(worksheet);
                
                Console.WriteLine("VBA module removed successfully for the specified worksheet.");
                
                // Modülün kaldırıldığını doğrulayın
                if (modules.Count == 0)
                {
                    Console.WriteLine("No VBA modules remain in the collection.");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Remove method: {ex.Message}");
            }
            
            // Sonucu kaydet
            workbook.Save("VbaModuleRemoveWithWorksheetDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## Remove(string) {#remove_1}

Modülü isimle kaldır

```csharp
public void Remove(string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| name | String |  |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodRemoveWithStringDemo
    {
        public static void Run()
        {
            // Makro içeren bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook();
            
            // VBA projesine erişin
            VbaProject vbaProject = workbook.VbaProject;
            
            // Yeni bir modül ekle
            int index = vbaProject.Modules.Add(VbaModuleType.Procedural, "TestModule");
            
            // Modüle bazı kodlar ekleyin
            vbaProject.Modules[index].Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";
            
            // Çalışma kitabını kaydedin
            workbook.Save("output_with_module.xlsm");
            
            // Modülü adını kullanarak kaldırın
            vbaProject.Modules.Remove("TestModule");
            
            // Kaldırma işleminden sonra çalışma kitabını kaydedin
            workbook.Save("output_after_removal.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


