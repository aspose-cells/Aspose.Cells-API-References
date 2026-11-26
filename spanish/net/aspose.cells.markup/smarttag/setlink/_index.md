---
title: "SmartTag.SetLink"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SmartTag. Cambia el nombre y el URI del espacio de nombres del smart tag"
type: docs
url: /es/net/aspose.cells.markup/smarttag/setlink/
---
## SmartTag.SetLink method

Cambia el nombre y el URI del espacio de nombres de la etiqueta inteligente.

```csharp
public void SetLink(string uri, string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uri | String | El URI del espacio de nombres del smart tag. |
| name | String | El nombre del smart tag. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagMethodSetLinkWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            workbook.Save("SmartTagSetLinkDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


