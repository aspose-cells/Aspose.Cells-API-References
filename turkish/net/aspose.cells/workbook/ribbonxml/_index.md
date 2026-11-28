---
title: "Workbook.RibbonXml"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Workbook özelliği. Ribbon UI'yi tanımlayan XML dosyasını alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells/workbook/ribbonxml/
---
## Workbook.RibbonXml property

Ribbon UI'yi tanımlayan XML dosyasını alır ve ayarlar.

```csharp
public string RibbonXml { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyRibbonXmlDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Ribbon'i özelleştirmek için örnek ribbon XML'i
            string ribbonXml = 
                "<customUI xmlns=\"http://schemas.microsoft.com/office/2006/01/customui\">" +
                "  <ribbon>" +
                "    <tabs>" +
                "      <tab id=\"customTab\" label=\"My Tab\">" +
                "        <group id=\"customGroup\" label=\"My Group\">" +
                "          <button id=\"customButton\" label=\"My Button\" size=\"large\" />" +
                "        </group>" +
                "      </tab>" +
                "    </tabs>" +
                "  </ribbon>" +
                "</customUI>";

            // RibbonXml özelliğini ayarla
            workbook.RibbonXml = ribbonXml;

            // Çalışma kitabını kaydedin
            workbook.Save("output.xlsm");

            // RibbonXml özelliğini doğrula
            Console.WriteLine("RibbonXml is set: " + (workbook.RibbonXml != null));
        }
    }
}
```

### Ayrıca Bakınız

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


