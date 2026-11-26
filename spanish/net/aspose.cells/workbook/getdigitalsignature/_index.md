---
title: "Workbook.GetDigitalSignature"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Workbook. Obtiene la firma digital del archivo"
type: docs
url: /es/net/aspose.cells/workbook/getdigitalsignature/
---
## Workbook.GetDigitalSignature method

Obtiene la firma digital del archivo.

```csharp
public DigitalSignatureCollection GetDigitalSignature()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.DigitalSignatures;
    using System;

    public class WorkbookMethodGetDigitalSignatureDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos para contexto
            worksheet.Cells["A1"].Value = "Sample Data";

            try
            {
                // Llame al método GetDigitalSignature para obtener firmas digitales
                DigitalSignatureCollection digitalSignatures = workbook.GetDigitalSignature();

                // Mostrar información sobre las firmas digitales
                if (digitalSignatures != null)
                {
                    int count = 0;
                    foreach (var signature in digitalSignatures)
                    {
                        count++;
                    }
                    Console.WriteLine("Number of digital signatures: " + count);
                    Console.WriteLine("GetDigitalSignature method called successfully");
                }
                else
                {
                    Console.WriteLine("No digital signatures found");
                }

                // Guarda el libro de trabajo
                workbook.Save("GetDigitalSignatureDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error calling GetDigitalSignature: " + ex.Message);
            }
        }
    }
}
```

### Ver también

* class [DigitalSignatureCollection](../../../aspose.cells.digitalsignatures/digitalsignaturecollection/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


