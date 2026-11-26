---
title: "ListObject.ShowTableStyleColumnStripes"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListObject. Indica si el formato de franjas de columna se aplica"
type: docs
url: /es/net/aspose.cells.tables/listobject/showtablestylecolumnstripes/
---
## ListObject.ShowTableStyleColumnStripes property

Indica si se aplica formato de franjas de columna.

```csharp
public bool ShowTableStyleColumnStripes { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyShowTableStyleColumnStripesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Mary");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Peter");
            worksheet.Cells["B4"].PutValue(35);

            // Crear un objeto de lista y obtener la referencia
            int listObjectIndex = worksheet.ListObjects.Add("A1", "B4", true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];
            
            // Establecer la propiedad de franjas de columna
            listObject.ShowTableStyleColumnStripes = true;
            
            // Guarda el libro de trabajo
            workbook.Save("ListObjectWithColumnStripes.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Workbook saved with column stripes enabled.");
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


