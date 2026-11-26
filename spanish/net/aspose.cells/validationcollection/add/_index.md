---
title: "ValidationCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ValidationCollection. Añade una validación de datos a la colección"
type: docs
url: /es/net/aspose.cells/validationcollection/add/
---
## Add() {#add}

Agrega una validación de datos a la colección.

```csharp
[Obsolete("Use ValidationCollection.Add(CellArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add()
```

### Valor de retorno

[`Validation`](../../validation/) object index.

### Observaciones

NOTA: Este método está ahora obsoleto. En su lugar, por favor use el método ValidationCollection.Add(CellArea). Este método será eliminado 12 meses después desde ENERO de 2015. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ver también

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

Agrega una validación de datos a la colección.

```csharp
public int Add(CellArea ca)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| ca | CellArea | El área contiene esta validación. |

### Valor de retorno

[`Validation`](../../validation/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodAddWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Crear un área de celdas para la validación
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 0;
            cellarea.StartColumn = 0;
            cellarea.EndRow = 1;
            cellarea.EndColumn = 1;
            
            // Agregar validación a la colección
            int index = sheet.Validations.Add(cellarea);
            Validation validation = sheet.Validations[index];
            
            // Configurar ajustes de validación
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AlertStyle = ValidationAlertType.Information;
            
            // Guarda el libro de trabajo
            workbook.Save("ValidationCollectionMethodAddWithCellAreaDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


