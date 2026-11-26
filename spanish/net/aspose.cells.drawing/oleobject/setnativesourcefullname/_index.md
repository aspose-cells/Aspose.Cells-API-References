---
title: "OleObject.SetNativeSourceFullName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método OleObject. Establece el nombre completo del archivo de origen nativo ole con ruta"
type: docs
url: /es/net/aspose.cells.drawing/oleobject/setnativesourcefullname/
---
## OleObject.SetNativeSourceFullName method

Establece el nombre completo del archivo nativo ole de origen con la ruta.

```csharp
public void SetNativeSourceFullName(string sourceFullName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| sourceFullName | String | el nombre completo del archivo de origen nativo ole |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class OleObjectMethodSetNativeSourceFullNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un OleObject a la hoja de cálculo
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]); // Changed to empty byte array
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Llame al método SetNativeSourceFullName con un parámetro de cadena
                oleObject.SetNativeSourceFullName(@"C:\temp\updated_test.xlsx");
                
                Console.WriteLine("SetNativeSourceFullName method executed successfully with parameter: C:\\temp\\updated_test.xlsx");
                
                // Muestre el efecto verificando la propiedad ObjectSourceFullName
                Console.WriteLine($"OleObject's source is now: {oleObject.ObjectSourceFullName}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetNativeSourceFullName method: {ex.Message}");
            }
            
            // Guarda el libro de trabajo
            workbook.Save("OleObjectMethodSetNativeSourceFullNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


