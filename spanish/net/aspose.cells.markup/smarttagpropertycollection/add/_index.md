---
title: "SmartTagPropertyCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SmartTagPropertyCollection. Añade una propiedad de la etiqueta inteligente de celdas"
type: docs
url: /es/net/aspose.cells.markup/smarttagpropertycollection/add/
---
## SmartTagPropertyCollection.Add method

Agrega una propiedad de la etiqueta inteligente de la celda.

```csharp
public int Add(string name, string value)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre de la propiedad |
| valor | String | El valor de la propiedad. |

### Valor de retorno

devuelve [`SmartTagProperty`](../../smarttagproperty/)

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagPropertyCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            smartTags.Add("http://docs.aspose.com", "docs");
            SmartTag smartTag = smartTags[0];

            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add("Author", "Aspose");
            properties.Add("Version", "1.0");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### Ver también

* class [SmartTagPropertyCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


