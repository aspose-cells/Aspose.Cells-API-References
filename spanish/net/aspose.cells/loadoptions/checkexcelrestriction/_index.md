---
title: "LoadOptions.CheckExcelRestriction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LoadOptions. Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite introducir un valor de cadena mayor a 32 K. Cuando introduces un valor mayor a 32 K, como mediante Cell.PutValuestring, si esta propiedad es verdadera obtendrás una excepción. Si la propiedad es falsa aceptaremos tu cadena de entrada como el valor de la celda, de modo que luego puedas exportar el valor completo de la cadena a otros formatos de archivo como CSV. Sin embargo, si estableces un valor que es inválido para el formato de archivo Excel, no deberías guardar el libro de trabajo como formato Excel más adelante. De lo contrario podría haber errores inesperados en el archivo Excel generado."
type: docs
url: /es/net/aspose.cells/loadoptions/checkexcelrestriction/
---
## LoadOptions.CheckExcelRestriction property

Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite introducir un valor de cadena superior a 32 K. Cuando introduces un valor superior a 32 K, como mediante Cell.PutValue(string), si esta propiedad es verdadera, obtendrás una excepción. Si esta propiedad es falsa, aceptaremos la cadena introducida como el valor de la celda, de modo que posteriormente puedas exportar la cadena completa a otros formatos de archivo como CSV. Sin embargo, si has establecido un valor que no es válido para el formato de archivo Excel, no deberías guardar el libro posteriormente en formato Excel. De lo contrario, podría producirse un error inesperado en el archivo Excel generado.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Desactivar la comprobación de restricciones de Excel
            workbook.Settings.CheckExcelRestriction = false;

            // Acceder a la primera hoja de cálculo y a sus celdas
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Crear una cadena más larga que el límite normal de Excel (32767 caracteres)
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // Colocar la cadena larga en la celda A1
            cells["A1"].PutValue(longString);
            
            // Guardar con la comprobación de restricciones desactivada
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;
            workbook.Save("output.xlsx", saveOptions);
            
            // Cargar con la comprobación de restricciones desactivada
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output.xlsx", loadOptions);
            
            // Verificar que la cadena larga se haya conservado
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("String length: " + loadedValue.Length);
            Console.WriteLine("String matches: " + loadedValue.Equals(longString));
        }
    }
}
```

### Ver también

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


