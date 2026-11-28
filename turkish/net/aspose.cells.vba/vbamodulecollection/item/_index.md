---
title: "VbaModuleCollection.Item"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaModuleCollection özelliği. Listedeki VbaModule'ü indeks ile alır"
type: docs
url: /tr/net/aspose.cells.vba/vbamodulecollection/item/
---
## VbaModuleCollection indexer (1 of 2)

Listedeki [`VbaModule`](../../vbamodule/) öğesini indeks ile alır.

```csharp
public VbaModule this[int index] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| indeks | İndeks. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // VBA projesi içeren yeni bir çalışma kitabı oluşturun
            Workbook workbook = new Workbook("sample.xlsm");
            
            // Mevcut VBA projesini alın (VbaProject yalnızca okunabilir)
            VbaProject vbaProject = workbook.VbaProject;
            
            // VBA projesine bir modül ekleyin
            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            
            // Modüle Item özelliğiyle erişin
            VbaModule module = vbaProject.Modules[index];
            
            // Modüle bazı VBA kodları ekleyin
            module.Codes = "Sub TestMacro()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            
            // Çalışma kitabını kaydedin
            workbook.Save("VbaModuleDemo.xlsm", SaveFormat.Xlsm);
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)

---

## VbaModuleCollection indexer (2 of 2)

Listedeki [`VbaModule`](../../vbamodule/) öğesini ad ile alır.

```csharp
public VbaModule this[string name] { get; }
```

| Parametre | Açıklama |
| --- | --- |
| name | Modülün adı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // Bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma kitabına VBA modülü ekleyin
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Modüle ad ile Item özelliği kullanarak erişin
            VbaModule module = workbook.VbaProject.Modules[worksheet.CodeName];
            
            // VBA kodunu ayarlayın
            module.Codes = "Sub Test()\r\n    MsgBox \"Hello World!\"\r\nEnd Sub";
            
            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
            
            // Geri yükleyerek doğrula
            Workbook verifyWorkbook = new Workbook("output.xlsm");
            VbaModule verifyModule = verifyWorkbook.VbaProject.Modules[worksheet.CodeName];
            
            Console.WriteLine("VBA Code in saved file:");
            Console.WriteLine(verifyModule.Codes);
        }
    }
}
```

### Ayrıca Bakınız

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


