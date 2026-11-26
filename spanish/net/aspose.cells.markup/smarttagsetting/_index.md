---
title: "Clase SmartTagSetting"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Markup.SmartTagSetting. Representa todos los objetos SmartTagCollection en la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.markup/smarttagsetting/
---
## SmartTagSetting class

Representa todos los objetos [`SmartTagCollection`](../smarttagcollection/) en la hoja de cálculo.

```csharp
public class SmartTagSetting : CollectionBase
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Item](../../aspose.cells.markup/smarttagsetting/item/) { get; } | Obtiene un objeto [`SmartTagCollection`](../smarttagcollection/) por el índice. (3 indexadores) |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add_1)(string) | Agrega una etiqueta inteligente a la celda. |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add)(int, int) | Agrega un objeto [`SmartTagCollection`](../smarttagcollection/) a una celda. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingDemo
    {
        public static void SmartTagSettingExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega una etiqueta inteligente a una celda específica
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Adding smart tag to cell A1

            // Acceda a la SmartTagCollection de la celda
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];

            // Agregue una smart tag a la colección
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            // Establezca la capacidad de la configuración de smart tag
            smartTagSetting.Capacity = 10;

            // Imprima el recuento de smart tags
            Console.WriteLine("Total Smart Tags: " + smartTagSetting.Count);

            // Guarda el libro de trabajo
            workbook.Save("SmartTagSettingExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


