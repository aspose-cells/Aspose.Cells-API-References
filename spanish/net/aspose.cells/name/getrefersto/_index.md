---
title: "Name.GetRefersTo"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Name. Obtenga la referencia de este Name"
type: docs
url: /es/net/aspose.cells/name/getrefersto/
---
## GetRefersTo(bool, bool) {#getrefersto}

Obtenga la referencia de este Name.

```csharp
public string GetRefersTo(bool isR1C1, bool isLocal)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | Booleano | Indica si la referencia necesita formatearse como R1C1. |
| isLocal | Booleano | Indica si la referencia necesita formatearse según la configuración regional. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodGetRefersToWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a las celdas
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");

            // Crear un rango con nombre
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";

            try
            {
                // Llame a GetRefersTo con formato R1C1 y alcance local
                string refersToR1C1Local = namedRange.GetRefersTo(true, true);
                Console.WriteLine("R1C1 format with local scope: " + refersToR1C1Local);

                // Llame a GetRefersTo con formato A1 y alcance global
                string refersToA1Global = namedRange.GetRefersTo(false, false);
                Console.WriteLine("A1 format with global scope: " + refersToA1Global);

                // Mostrar los detalles del rango con nombre
                Console.WriteLine("Named range text: " + namedRange.Text);
                Console.WriteLine("Full text: " + namedRange.FullText);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("NameMethodGetRefersToDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetRefersTo(bool, bool, int, int) {#getrefersto_1}

Obtenga la referencia de este Name basada en la celda especificada.

```csharp
public string GetRefersTo(bool isR1C1, bool isLocal, int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| isR1C1 | Booleano | Indica si la referencia necesita formatearse como R1C1. |
| isLocal | Booleano | Indica si la referencia necesita formatearse según la configuración regional. |
| fila | Int32 | El índice de fila de la celda. |
| columna | Int32 | El índice de columna de la celda. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a las celdas
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);

            // Crear un rango con nombre
            int index = workbook.Worksheets.Names.Add("MyNamedRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$A$3";

            try
            {
                // Llame a GetRefersTo con parámetros específicos (isR1C1, isLocal, row, column)
                string refersTo = namedRange.GetRefersTo(false, false, 0, 0);
                
                Console.WriteLine("Named range refers to: " + refersTo);
                Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean, Int32, Int32)");

                // Modificar el rango con nombre basado en el resultado
                if (!string.IsNullOrEmpty(refersTo))
                {
                    worksheet.Cells["B1"].PutValue("Named Range Refers To:");
                    worksheet.Cells["B2"].PutValue(refersTo);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


