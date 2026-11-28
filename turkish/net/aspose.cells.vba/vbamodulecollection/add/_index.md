---
title: "VbaModuleCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "VbaModuleCollection yöntemi. Bir çalışma sayfası için modül ekler"
type: docs
url: /tr/net/aspose.cells.vba/vbamodulecollection/add/
---
## Add(Worksheet) {#add_1}

Bir çalışma sayfası için modül ekler.

```csharp
public int Add(Worksheet sheet)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sayfa | Çalışma Sayfası | Çalışma sayfası |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithWorksheetDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // İlk çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Çalışma sayfasıyla ilişkili bir VBA modülü ekleyin
            int moduleIndex = workbook.VbaProject.Modules.Add(worksheet);
            
            // Modüle bazı VBA kodları ekleyin
            string vbaCode = "Sub Test()\n    MsgBox \"Hello from VBA!\"\nEnd Sub";
            workbook.VbaProject.Modules[moduleIndex].Codes = vbaCode;
            
            // VBA projesiyle birlikte çalışma kitabını kaydedin
            workbook.Save("output.xlsm", SaveFormat.Xlsm);
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

## Add(VbaModuleType, string) {#add}

Modül ekler.

```csharp
public int Add(VbaModuleType type, string name)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | VbaModuleType | Modülün türü. |
| name | String | Modülün adı. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;

namespace AsposeCellsExamples
{
    public class VbaModuleCollectionMethodAddWithVbaModuleTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            VbaProject vbaProject = workbook.VbaProject;

            int index = vbaProject.Modules.Add(VbaModuleType.Class, "TestModule");
            VbaModule module = vbaProject.Modules[index];
            module.Codes = "Sub Test()\r\nMsgBox \"Hello World\"\r\nEnd Sub";

            workbook.Save("VbaModuleAddExample.xlsm");
        }
    }
}
```

### Ayrıca Bakınız

* enum [VbaModuleType](../../vbamoduletype/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)


