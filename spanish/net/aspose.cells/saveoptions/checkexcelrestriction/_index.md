---
title: "SaveOptions.CheckExcelRestriction"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SaveOptions. Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite introducir un valor de cadena mayor a 32 K. Cuando se introduce un valor mayor a 32 K se truncará"
type: docs
url: /es/net/aspose.cells/saveoptions/checkexcelrestriction/
---
## SaveOptions.CheckExcelRestriction property

Indica si se verifica la restricción del archivo Excel cuando el usuario modifica objetos relacionados con celdas. Por ejemplo, Excel no permite ingresar un valor de cadena mayor a 32K. Cuando se ingresa un valor mayor a 32K, se truncará.

```csharp
public bool CheckExcelRestriction { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyCheckExcelRestrictionDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Desactivar la verificación de restricciones de Excel
            workbook.Settings.CheckExcelRestriction = false;

            // Acceder a la primera hoja de cálculo y a sus celdas
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Crear una cadena más larga que el límite normal de Excel
            string longString = new string('x', 32767) + " Testing Excel restriction";
            
            // Colocar la cadena larga en la celda A1
            cells["A1"].PutValue(longString);

            // Configurar las opciones de guardado para omitir las restricciones
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CheckExcelRestriction = false;

            // Guarda el libro de trabajo
            workbook.Save("output_without_restrictions.xlsx", saveOptions);

            // Cargar el archivo guardado con las restricciones desactivadas
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.CheckExcelRestriction = false;
            Workbook loadedWorkbook = new Workbook("output_without_restrictions.xlsx", loadOptions);

            // Verificar que la cadena larga se haya conservado
            string loadedValue = loadedWorkbook.Worksheets[0].Cells["A1"].StringValue;
            Console.WriteLine("Loaded string length: " + loadedValue.Length);
            Console.WriteLine("First 50 chars: " + loadedValue.Substring(0, 50));
            Console.WriteLine("Last 50 chars: " + loadedValue.Substring(loadedValue.Length - 50));
        }
    }
}
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


