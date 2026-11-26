---
title: "AbstractLowCodeProtectionProvider.GetWorksheetProtectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método AbstractLowCodeProtectionProvider. Obtiene el tipo de protección para proteger la hoja de cálculo especificada"
type: docs
url: /es/net/aspose.cells.lowcode/abstractlowcodeprotectionprovider/getworksheetprotectiontype/
---
## AbstractLowCodeProtectionProvider.GetWorksheetProtectionType method

Obtiene el tipo de protección para proteger la hoja de cálculo especificada.

```csharp
public virtual ProtectionType GetWorksheetProtectionType(string sheetName)
```

### Valor de retorno

Tipo de protección para proteger la hoja de cálculo especificada. Ninguno significa que no hay protección para la hoja.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class AbstractLowCodeProtectionProviderMethodGetWorksheetProtectionTypeWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("newSheet");
            string name = worksheet.Name;
            var protectionProvider = new CustomProtectionProvider();

            try
            {
                worksheet.Protect(protectionProvider.GetWorksheetProtectionType(name), protectionProvider.GetWorksheetPassword(name), "");
               
                // Mostrar el resultado
                Console.WriteLine($"Worksheet '{name}' protection type: {protectionProvider.GetWorksheetProtectionType(name)}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error retrieving protection type: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("GetWorksheetProtectionTypeDemo.xlsx");
        }

        private class CustomProtectionProvider : AbstractLowCodeProtectionProvider
        {
            public override ProtectionType GetWorksheetProtectionType(string sheetName)
            {
                return ProtectionType.Structure;
            }

            public override string GetWorksheetPassword(string sheetName)
            {
                return $"aspose123_{sheetName}";
            }
        }

    }
    
}
```

### Ver también

* enum [ProtectionType](../../../aspose.cells/protectiontype/)
* class [AbstractLowCodeProtectionProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


