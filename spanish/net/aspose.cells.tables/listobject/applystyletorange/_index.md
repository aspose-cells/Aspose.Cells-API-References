---
title: "ListObject.ApplyStyleToRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ListObject. Aplicar el estilo de tabla al rango"
type: docs
url: /es/net/aspose.cells.tables/listobject/applystyletorange/
---
## ListObject.ApplyStyleToRange method

Aplica el estilo de tabla al rango.

```csharp
public void ApplyStyleToRange()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectMethodApplyStyleToRangeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue datos de ejemplo para crear un objeto de lista
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crear un objeto de lista
            int index = worksheet.ListObjects.Add("A1", "B3", true);
            ListObject listObject = worksheet.ListObjects[index];

            // Aplicar estilo al rango del objeto de lista
            listObject.ApplyStyleToRange();

            // Verificar que el estilo se aplicó comprobando el color de primer plano de una celda
            Style style = worksheet.Cells["A1"].GetStyle();
            Console.WriteLine("Foreground color applied: " + style.ForegroundColor);

            // Convertir el objeto de lista a rango y verificar
            listObject.ConvertToRange();
            Console.WriteLine("List objects count after conversion: " + worksheet.ListObjects.Count);
        }
    }
}
```

### Ver también

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


