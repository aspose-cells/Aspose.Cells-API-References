---
title: "WorksheetCollection.Insert"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Insertar una hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheetcollection/insert/
---
## Insert(int, SheetType) {#insert}

Insertar una hoja de cálculo.

```csharp
public Worksheet Insert(int index, SheetType sheetType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice de la hoja |
| sheetType | SheetType | El tipo de hoja. |

### Valor de retorno

Devuelve una hoja de cálculo insertada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Insert(1, SheetType.Worksheet);
            worksheet.Name = "InsertedSheet";
            workbook.Worksheets[0].Cells["A1"].Value = "Referencing inserted sheet:";
            workbook.Worksheets[0].Cells["A2"].Formula = "='InsertedSheet'!A1";
        }
    }
}
```

### Ver también

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Insert(int, SheetType, string) {#insert_1}

Insertar una hoja de cálculo.

```csharp
public Worksheet Insert(int index, SheetType sheetType, string sheetName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice de la hoja |
| sheetType | SheetType | El tipo de hoja. |
| sheetName | String | El nombre de la hoja. |

### Valor de retorno

Devuelve una hoja de cálculo insertada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodInsertWithInt32SheetTypeStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Insertar una nueva hoja de cálculo en el índice 0 con el nombre "InsertedSheet"
            workbook.Worksheets.Insert(0, SheetType.Worksheet, "InsertedSheet");
            
            // Acceder a la hoja de cálculo insertada
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Colocar algunos datos en la celda A1 de la hoja insertada
            worksheet.Cells["A1"].PutValue("This sheet was inserted using Insert method");
            
            // Guarda el libro de trabajo
            workbook.Save("WorksheetInsertDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


