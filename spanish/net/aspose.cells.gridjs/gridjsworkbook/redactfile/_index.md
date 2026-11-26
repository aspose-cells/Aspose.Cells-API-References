---
title: "GridJsWorkbook.RedactFile"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GridJsWorkbook. Realiza la redacción en un archivo Excel basado en una matriz de operaciones JSON."
type: docs
url: /es/net/aspose.cells.gridjs/gridjsworkbook/redactfile/
---
## GridJsWorkbook.RedactFile method

Realiza una redacción en un archivo Excel basada en una matriz de operaciones JSON.

```csharp
public void RedactFile(string excelFilePath, string uid, string[] arrayOfRedactionOpr)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| excelFilePath | String | La ruta del archivo Excel a redactar. |
| uid | String | El identificador único para el libro. Si es null o está vacío, se generará un nuevo uid basado en la ruta del archivo. |
| arrayOfRedactionOpr | String[] | Una matriz de cadenas JSON que representan las operaciones de redacción a aplicar. |

### Excepciones

| excepción | condición |
| --- | --- |
| [GridCellException](../../gridcellexception/) | Se lanza cuando ocurre una CellsException durante la operación de redacción. |
| Exception | Se lanza cuando ocurre una excepción general durante la operación de redacción. |

### Ver también

* class [GridJsWorkbook](../)
* namespace [Aspose.Cells.GridJs](../../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../../)


