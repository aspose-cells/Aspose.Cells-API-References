---
title: "WorksheetCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Elimina el elemento con un nombre especificado"
type: docs
url: /es/net/aspose.cells/worksheetcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Elimina el elemento con un nombre especificado.

```csharp
public void RemoveAt(string name)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | El nombre del elemento a eliminar. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Agregar algunas hojas de cálculo
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");
            
            // Agregar un rango con nombre (fijo)
            int nameIndex = wb.Worksheets.Names.Add("testname");
            wb.Worksheets.Names[nameIndex].RefersTo = "=[Book1.xlsx]Sheet1!$A1";
            
            // Demostrar RemoveAt con parámetro de cadena
            Console.WriteLine($"Before removal - Worksheet count: {wb.Worksheets.Count}");
            wb.Worksheets.RemoveAt("Sheet1");
            Console.WriteLine($"After removal - Worksheet count: {wb.Worksheets.Count}");
            
            // Guarda el libro de trabajo
            using (MemoryStream ms = new MemoryStream())
            {
                wb.Save(ms, SaveFormat.Xlsx);
            }
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int) {#removeat}

Elimina el elemento en un índice especificado.

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El valor del índice del elemento a eliminar. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            
            // Agregar algunas hojas de cálculo
            wb.Worksheets.Add("Sheet1");
            wb.Worksheets.Add("Sheet2");
            wb.Worksheets.Add("Sheet3");

            // Mostrar el recuento original de hojas de cálculo
            Console.WriteLine($"Original worksheet count: {wb.Worksheets.Count}");

            // Eliminar hoja de cálculo en el índice 1 (segunda hoja)
            wb.Worksheets.RemoveAt(1);

            // Mostrar el recuento actualizado de hojas de cálculo
            Console.WriteLine($"After removal, worksheet count: {wb.Worksheets.Count}");

            // Guarda el libro de trabajo
            wb.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


