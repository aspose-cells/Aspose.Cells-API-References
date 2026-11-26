---
title: "SmartTagSetting.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SmartTagSetting. Añade un objeto SmartTagCollection a una celda"
type: docs
url: /es/net/aspose.cells.markup/smarttagsetting/add/
---
## Add(int, int) {#add}

Añade un objeto [`SmartTagCollection`](../../smarttagcollection/) a una celda.

```csharp
public int Add(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | La fila de la celda. |
| columna | Int32 | La columna de la celda. |

### Valor de retorno

Devuelve el índice de un objeto [`SmartTagCollection`](../../smarttagcollection/) en la hoja de cálculo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;

namespace AsposeCellsExamples
{
    public class SmartTagSettingMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Add to cell A1 (row 0, column 0)

            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];
            smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            Console.WriteLine("Smart Tags Count: " + smartTagSetting.Count.ToString());
            workbook.Save("SmartTagDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Agrega una etiqueta inteligente a la celda.

```csharp
public int Add(string cellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | El nombre de la celda. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingMethodAddWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Obtenga la instancia SmartTagSetting
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            
            try
            {
                // Llame al método Add con un parámetro String
                int index = smartTagSetting.Add("A1");
                
                Console.WriteLine($"SmartTag added successfully at index: {index}");
                
                // Añade contenido para demostrar el efecto
                worksheet.Cells["A1"].PutValue("This cell has a smart tag");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("SmartTagSettingMethodAddWithStringDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SmartTagSetting](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


