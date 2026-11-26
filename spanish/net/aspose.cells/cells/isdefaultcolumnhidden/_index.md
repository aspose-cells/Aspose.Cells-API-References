---
title: "Cells.IsDefaultColumnHidden"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Cells."
type: docs
url: /es/net/aspose.cells/cells/isdefaultcolumnhidden/
---
## Cells.IsDefaultColumnHidden property

```csharp
public bool IsDefaultColumnHidden { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultColumnHiddenDemo
    {
        public static void Run()
        {
            try
            {
                // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];
                Cells cells = worksheet.Cells;

                // Agrega algunos datos para que la hoja de cálculo no esté vacía
                cells["A1"].PutValue("First");
                cells["B1"].PutValue("Second");
                cells["C1"].PutValue("Third");

                // Lee la propiedad IsDefaultColumnHidden (el valor predeterminado es false)
                bool isDefaultColumnHidden = cells.IsDefaultColumnHidden;
                Console.WriteLine("IsDefaultColumnHidden: " + isDefaultColumnHidden);

                // Guarda el libro de trabajo (opcional, solo para completar la demostración)
                workbook.Save("IsDefaultColumnHiddenDemo.xlsx", SaveFormat.Xlsx);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


