---
title: "OdsSaveOptions.IsStrictSchema11"
second_title: "Aspose.Cells için .NET API Referansı"
description: "OdsSaveOptions özelliği. ODS dosyasının ODF formatı sürüm 1.1 olarak kaydedilip kaydedilmeyeceğini gösterir. Varsayılan false'tur"
type: docs
url: /tr/net/aspose.cells/odssaveoptions/isstrictschema11/
---
## OdsSaveOptions.IsStrictSchema11 property

ODS dosyasının ODF formatı sürüm 1.1 olarak kaydedilip kaydedilmeyeceğini gösterir. Varsayılan false'tur.

```csharp
[Obsolete("Use OdsSaveOptions.OdfStrictVersion property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsStrictSchema11 { get; set; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen OdsSaveOptions.OdfStrictVersion özelliğini kullanın. Bu yöntem, Şubat 2024'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OdsSaveOptionsPropertyIsStrictSchema11Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample ODS with strict schema");

            OdsSaveOptions saveOptions = new OdsSaveOptions();
            saveOptions.IsStrictSchema11 = true;
            
            workbook.Save("StrictSchema11Example.ods", saveOptions);
        }
    }
}
```

### Ayrıca Bakınız

* class [OdsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


