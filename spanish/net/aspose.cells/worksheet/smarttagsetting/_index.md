---
title: "Worksheet.SmartTagSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Worksheet propiedad. Obtiene todos los objetos SmartTagCollection de la hoja"
type: docs
url: /es/net/aspose.cells/worksheet/smarttagsetting/
---
## Worksheet.SmartTagSetting property

Obtiene todos los objetos [`SmartTagCollection`](../../../aspose.cells.markup/smarttagcollection/) de la hoja.

```csharp
public SmartTagSetting SmartTagSetting { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class WorksheetPropertySmartTagSettingDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart Tags Count: " + smartTagSetting.Count.ToString());

            workbook.Save("SmartTagSettingDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SmartTagSetting](../../../aspose.cells.markup/smarttagsetting/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


