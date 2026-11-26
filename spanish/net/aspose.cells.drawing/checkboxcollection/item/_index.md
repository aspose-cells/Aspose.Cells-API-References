---
title: "CheckBoxCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CheckBoxCollection. Obtiene el elemento CheckBox en el índice especificado"
type: docs
url: /es/net/aspose.cells.drawing/checkboxcollection/item/
---
## CheckBoxCollection indexer

Obtiene el elemento [`CheckBox`](../../checkbox/) en el índice especificado.

```csharp
public CheckBox this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CheckBoxCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar un checkbox a la hoja de cálculo
            int index = worksheet.CheckBoxes.Add(10, 10, 100, 20);
            
            // Accede al checkbox usando la propiedad Item (indexador)
            Aspose.Cells.Drawing.CheckBox checkBox = worksheet.CheckBoxes[index];
            checkBox.Text = "Sample CheckBox";
            checkBox.Name = "CheckBox1";
            
            // Accede al checkbox usando el índice (propiedad Item)
            Aspose.Cells.Drawing.CheckBox checkBoxByName = worksheet.CheckBoxes[0];
            
            // Muestra las propiedades del checkbox
            Console.WriteLine("CheckBox Name: " + checkBoxByName.Name);
            Console.WriteLine("CheckBox Text: " + checkBoxByName.Text);
            
            // Guarda el libro de trabajo
            workbook.Save("CheckBoxExample.xlsx");
        }
    }
}
```

### Ver también

* class [CheckBox](../../checkbox/)
* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


