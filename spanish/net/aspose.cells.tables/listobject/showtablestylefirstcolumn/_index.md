---
title: "ListObject.ShowTableStyleFirstColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Indica si la primera columna de la tabla es a la que se aplica el estilo"
type: docs
url: /es/net/aspose.cells.tables/listobject/showtablestylefirstcolumn/
---
## ListObject.ShowTableStyleFirstColumn property

Indica si la primera columna de la tabla tiene el estilo aplicado.

```csharp
public bool ShowTableStyleFirstColumn { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleFirstColumnDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["B3"].PutValue(1.8);
            worksheet.Cells["B4"].PutValue(3.2);

            // Crear un objeto de lista
            ListObjectCollection listObjects = worksheet.ListObjects;
            int index = listObjects.Add("A1", "B4", true);
            ListObject listObject = listObjects[index];
            
            // Aplicar estilo a la primera columna
            listObject.ShowTableStyleFirstColumn = true;
            
            // Guarda el libro de trabajo
            workbook.Save("ListObjectShowFirstColumnStyle.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("File saved with first column style applied to the table.");
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


