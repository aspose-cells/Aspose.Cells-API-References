---
title: "SmartTagCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SmartTagCollection. Añade una etiqueta inteligente"
type: docs
url: /es/net/aspose.cells.markup/smarttagcollection/add/
---
## SmartTagCollection.Add method

Agrega una smart tag.

```csharp
public int Add(string uri, string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| uri | String | Especifica el URI del espacio de nombres de la etiqueta inteligente |
| name | String | Especifica el nombre de la etiqueta inteligente. |

### Valor de retorno

El índice de la etiqueta inteligente en la lista.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagCollectionMethodAddWithStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Added smart tag at index: " + tagIndex);
            workbook.Save("SmartTagCollectionAddExample.xlsx");
        }
    }
}
```

### Ver también

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


