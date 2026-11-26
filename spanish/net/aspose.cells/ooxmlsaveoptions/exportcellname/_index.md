---
title: "OoxmlSaveOptions.ExportCellName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad OoxmlSaveOptions. Indica si exportar el nombre de la celda a un archivo Excel2007 .xlsx .xlsm .xltx .xltm. Si el archivo de salida puede ser accedido por SQL Server DTS, este valor debe ser verdadero. Establecer el valor a false aumentará considerablemente el rendimiento y reducirá el tamaño del archivo al crear archivos grandes. El valor predeterminado es true."
type: docs
url: /es/net/aspose.cells/ooxmlsaveoptions/exportcellname/
---
## OoxmlSaveOptions.ExportCellName property

Indica si se exporta el nombre de la celda a un archivo Excel2007 .xlsx (.xlsm, .xltx, .xltm). Si el archivo de salida puede ser accedido por SQL Server DTS, este valor debe ser verdadero. Configurar el valor a falso aumentará considerablemente el rendimiento y reducirá el tamaño del archivo al crear archivos grandes. El valor predeterminado es verdadero.

```csharp
public bool ExportCellName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyExportCellNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Colocar algunos datos en las celdas
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            
            // Crear opciones de guardado XLSX con ExportCellName habilitado
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.ExportCellName = true;
            
            // Guardar el libro de trabajo con los nombres de celda exportados
            workbook.Save("output_with_cellnames.xlsx", saveOptions);
            
            // Crear otras opciones de guardado con ExportCellName deshabilitado (predeterminado)
            OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
            
            // Guardar el libro de trabajo sin exportar los nombres de celda
            workbook.Save("output_without_cellnames.xlsx", saveOptions2);
        }
    }
}
```

### Ver también

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


