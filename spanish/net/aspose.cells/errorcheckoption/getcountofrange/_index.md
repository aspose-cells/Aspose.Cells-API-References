---
title: "ErrorCheckOption.GetCountOfRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ErrorCheckOption method. Obtiene el recuento de rangos que fueron influenciados por esta configuración"
type: docs
url: /es/net/aspose.cells/errorcheckoption/getcountofrange/
---
## ErrorCheckOption.GetCountOfRange method

Obtiene el recuento de rangos influenciados por esta configuración.

```csharp
public int GetCountOfRange()
```

### Valor de retorno

el recuento de rangos que fueron influenciados por esta configuración.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ErrorCheckOptionMethodGetCountOfRangeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Obtener colección de opciones de verificación de errores
            ErrorCheckOptionCollection optsCollection = sheet.ErrorCheckOptions;

            // Agregar primera opción de verificación de errores
            int index1 = optsCollection.Add();
            ErrorCheckOption opts1 = optsCollection[index1];
            opts1.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            opts1.AddRange(CellArea.CreateCellArea("A1", "D2"));
            opts1.AddRange(CellArea.CreateCellArea("A3", "D3"));

            // Agregar segunda opción de verificación de errores
            int index2 = optsCollection.Add();
            ErrorCheckOption opts2 = optsCollection[index2];
            opts2.SetErrorCheck(ErrorCheckType.TwoDigitTextYear, false);
            opts2.AddRange(CellArea.CreateCellArea("A3", "D5"));

            // Demostrar el método GetCountOfRange
            Console.WriteLine("First option range count: " + opts1.GetCountOfRange());
            Console.WriteLine("Second option range count: " + opts2.GetCountOfRange());

            // Guarda el libro de trabajo
            workbook.Save("ErrorCheckOptionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ErrorCheckOption](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


