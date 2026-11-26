---
title: "Clase SmartTag"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Markup.SmartTag. Representa una etiqueta inteligente"
type: docs
url: /es/net/aspose.cells.markup/smarttag/
---
## SmartTag class

Representa una etiqueta inteligente.

```csharp
public class SmartTag
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Deleted](../../aspose.cells.markup/smarttag/deleted/) { get; set; } | Indica si la etiqueta inteligente está eliminada. |
| [Name](../../aspose.cells.markup/smarttag/name/) { get; } | Obtiene el nombre de la etiqueta inteligente. |
| [Properties](../../aspose.cells.markup/smarttag/properties/) { get; set; } | Obtiene y establece las propiedades de la etiqueta inteligente. |
| [Uri](../../aspose.cells.markup/smarttag/uri/) { get; } | Obtiene el URI del espacio de nombres de la etiqueta inteligente. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [SetLink](../../aspose.cells.markup/smarttag/setlink/)(string, string) | Cambia el nombre y el URI del espacio de nombres de la etiqueta inteligente. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class MarkupClassSmartTagDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Description", "Aspose.Cells SmartTag");

            workbook.Save("SmartTagDemo.xlsx");
            Console.WriteLine("SmartTagDemo.xlsx created successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


