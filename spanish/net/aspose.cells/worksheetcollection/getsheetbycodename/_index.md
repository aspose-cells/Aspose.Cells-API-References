---
title: "WorksheetCollection.GetSheetByCodeName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Obtiene la hoja de cálculo por el nombre de código"
type: docs
url: /es/net/aspose.cells/worksheetcollection/getsheetbycodename/
---
## WorksheetCollection.GetSheetByCodeName method

Obtiene la hoja de cálculo por el nombre de código.

```csharp
public Worksheet GetSheetByCodeName(string codeName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| codeName | String | Nombre de código de la hoja de cálculo. |

### Valor de retorno

El elemento con el nombre de código especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodGetSheetByCodeNameWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar hojas de cálculo y establecer sus nombres de código
            Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
            sheet1.CodeName = "MainSheet";
            
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            sheet2.CodeName = "DataSheet";

            // Obtener hoja de cálculo por nombre de código
            Worksheet mainSheet = workbook.Worksheets.GetSheetByCodeName("MainSheet");
            Worksheet dataSheet = workbook.Worksheets.GetSheetByCodeName("DataSheet");

            // Demostrar el uso escribiendo en celdas
            mainSheet.Cells["A1"].PutValue("This is Main Sheet");
            dataSheet.Cells["A1"].PutValue("This is Data Sheet");

            // Guarda el libro de trabajo
            workbook.Save("GetSheetByCodeNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


