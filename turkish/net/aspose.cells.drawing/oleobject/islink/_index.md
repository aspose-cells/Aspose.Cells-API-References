---
title: "OleObject.IsLink"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OleObject özelliği. OleObject dosyaya bağlanıyorsa true döndürür"
type: docs
url: /tr/net/aspose.cells.drawing/oleobject/islink/
---
## OleObject.IsLink property

OleObject dosyaya bağlanıyorsa true döndürür.

```csharp
public bool IsLink { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OleObjectPropertyIsLinkDemo
    {
        public static void Run()
        {
            // Kaynak çalışma kitabını yükle
            Workbook workbook = new Workbook("example.xlsm");

            // Her çalışma sayfasını işleyin
            foreach (Worksheet worksheet in workbook.Worksheets)
            {
                // Çalışma sayfasındaki her OLE nesnesini işleyin
                foreach (Aspose.Cells.Drawing.OleObject ole in worksheet.OleObjects)
                {
                    // Bağlı değilse OLE nesnesini atlayın
                    if (!ole.IsLink)
                    {
                        Console.WriteLine("Skipping embedded OLE object");
                        continue;
                    }

                    // Bağlı dosya yolunu gösterin ve değiştirin
                    Console.WriteLine("Original linked file: " + ole.ObjectSourceFullName);
                    string newPath = ole.ObjectSourceFullName.Replace("C:", "D:");
                    ole.ObjectSourceFullName = newPath;
                    Console.WriteLine("Modified linked file: " + ole.ObjectSourceFullName);
                }
            }

            // Değiştirilmiş çalışma kitabını kaydet
            workbook.Save("modified_example.xlsm");
            Console.WriteLine("File saved with updated OLE links.");
        }
    }
}
```

### Ayrıca Bakınız

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


