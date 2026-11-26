---
title: "SmartTagSetting.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SmartTagSetting. Obtiene un objeto SmartTagCollection por el índice"
type: docs
url: /es/net/aspose.cells.markup/smarttagsetting/item/
---
## SmartTagSetting indexer (1 of 3)

Obtiene un objeto [`SmartTagCollection`](../../smarttagcollection/) por el índice.

```csharp
public SmartTagCollection this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| index | El índice del objeto [`SmartTagCollection`](../../smarttagcollection/) en la lista. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo1
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            sheet.Cells["A1"].PutValue("Aspose");
            sheet.Cells["A2"].PutValue("Cells");

            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0);
            
            // Demostrar el uso de la propiedad Item
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
            smartTags.Add("http://docs.aspose.com", "docs");
            
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink("http://www.aspose.com", "AsposeLink");

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

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (2 of 3)

Obtiene el objeto [`SmartTagCollection`](../../smarttagcollection/) de la celda.

```csharp
public SmartTagCollection this[int row, int column] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| fila | El índice de fila de la celda. |
| columna | El índice de columna de la celda |

### Valor de retorno

Devuelve el objeto [`SmartTagCollection`](../../smarttagcollection/) de la celda. Devuelve null si no hay etiquetas inteligentes en la celda.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingPropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            smartTagSetting.Add(0, 0); // Add smart tag to cell A1

            // Demostrar el uso de la propiedad Item
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart tags in cell A1: " + smartTagCollection.Count);
            Console.WriteLine("Namespace URI: " + smartTagCollection[0].Uri);
            Console.WriteLine("Tag name: " + smartTagCollection[0].Name);

            workbook.Save("SmartTagDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## SmartTagSetting indexer (3 of 3)

Obtiene el objeto [`SmartTagCollection`](../../smarttagcollection/) de la celda.

```csharp
public SmartTagCollection this[string cellName] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| cellName | El nombre de la celda. |

### Valor de retorno

Devuelve el objeto [`SmartTagCollection`](../../smarttagcollection/) de la celda. Devuelve null si no hay etiquetas inteligentes en la celda.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingPropertyItemDemo2
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Obtener la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Acceda al SmartTagSetting de la hoja de cálculo
                SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;

                // Añade una etiqueta inteligente a la celda A1 (fila 0, columna 0)
                int smartTagIndex = smartTagSetting.Add(0, 0);

                // Demuestra el uso de la propiedad Item (indexador)
                SmartTagCollection smartTagCollection = smartTagSetting[smartTagIndex];

                // Agregue una smart tag a la colección
                smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

                // Muestra información sobre la etiqueta inteligente
                Console.WriteLine("Number of smart tags in collection: " + smartTagCollection.Count);
                if (smartTagCollection.Count > 0)
                {
                    Console.WriteLine("First smart tag URI: " + smartTagCollection[0].Uri);
                    Console.WriteLine("First smart tag name: " + smartTagCollection[0].Name);
                }

                // Guarda el libro de trabajo
                workbook.Save("SmartTagItemDemo.xlsx");
                Console.WriteLine("SmartTagItemDemo.xlsx created successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SmartTagCollection](../../smarttagcollection/)
* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


