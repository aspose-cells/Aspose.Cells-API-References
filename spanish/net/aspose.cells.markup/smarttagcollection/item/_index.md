---
title: "SmartTagCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SmartTagCollection. Obtiene un objeto SmartTag en el índice específico"
type: docs
url: /es/net/aspose.cells.markup/smarttagcollection/item/
---
## SmartTagCollection indexer

Obtiene un objeto [`SmartTag`](../../smarttag/) en el índice específico

```csharp
public SmartTag this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice. |

### Valor de retorno

devuelve un objeto [`SmartTag`](../../smarttag/).

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagCollectionPropertyItemDemo
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

            // Demostrar el uso de la propiedad Item
            SmartTagProperty authorProperty = properties["Author"];
            Console.WriteLine($"Property 'Author' value: {authorProperty.Value}");

            workbook.Save("SmartTagPropertyDemo.xlsx");
            Console.WriteLine("SmartTagPropertyDemo.xlsx created successfully.");
        }
    }
}
```

### Ver también

* class [SmartTag](../../smarttag/)
* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


