---
title: "Workbook.RemoveMacro"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook yöntemi. Bu elektronik tablodan VBA/makroyu kaldırır"
type: docs
url: /tr/net/aspose.cells/workbook/removemacro/
---
## Workbook.RemoveMacro method

Bu elektronik tablodan VBA/makroyu kaldırır.

```csharp
public void RemoveMacro()
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodRemoveMacroDemo
    {
        public static void Run()
        {
            // Makro etkin bir dosyadan bir çalışma kitabı oluştur
            Workbook workbook = new Workbook("example.xlsm");

            // Çalışma kitabından makroları kaldır
            workbook.RemoveMacro();
            
            // Makrosuz çalışma kitabı olarak kaydet
            string noMacroPath = "NoMacro.xlsx";
            workbook.Save(noMacroPath, SaveFormat.Xlsx);

            Console.WriteLine("Macros removed successfully. File created: " + noMacroPath);
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


