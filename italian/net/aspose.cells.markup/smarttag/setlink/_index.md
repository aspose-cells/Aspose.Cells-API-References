---
title: "SmartTag.SetLink"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SmartTag. Cambia il nome e l'URI dello spazio dei nomi del tag intelligente"
type: docs
url: /it/net/aspose.cells.markup/smarttag/setlink/
---
## SmartTag.SetLink method

Modifica il nome e l'URI dello spazio dei nomi dello smart tag.

```csharp
public void SetLink(string uri, string name)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| uri | String | L'URI dello spazio dei nomi del tag intelligente. |
| name | String | Il nome del tag intelligente. |

### Esempi

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

### Vedi anche

* class [SmartTag](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


