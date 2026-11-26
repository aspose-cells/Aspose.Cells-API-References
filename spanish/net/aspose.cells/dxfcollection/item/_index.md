---
title: "DxfCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DxfCollection. Obtiene el elemento en el índice especificado"
type: docs
url: /es/net/aspose.cells/dxfcollection/item/
---
## DxfCollection indexer

Obtiene el elemento en el índice especificado.

```csharp
public Style this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice especificado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DxfCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Acceder a DxfCollection desde el libro de trabajo
            DxfCollection dxfCollection = workbook.Worksheets.Dxfs;

            // Crear un nuevo estilo (no se puede agregar directamente a DxfCollection ya que no tiene método Add)
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            // El estilo se agrega automáticamente a la colección al crearse

            // Obtener el primer elemento de DxfCollection usando la propiedad Item
            Style firstStyle = dxfCollection[0];
            Console.WriteLine("First style font name: " + firstStyle.Font.Name);

            // Modifique el estilo a través de la propiedad Item (ya que devuelve una referencia)
            firstStyle.Font.Color = System.Drawing.Color.Red;
            firstStyle.Font.IsBold = true;

            // Verificar el cambio
            Console.WriteLine("Modified style font color: " + dxfCollection[0].Font.Color);
            Console.WriteLine("Modified style font bold: " + dxfCollection[0].Font.IsBold);

            // Aplique el estilo a una celda para ver el efecto
            worksheet.Cells["A1"].PutValue("DxfCollection Property Item Demo");
            worksheet.Cells["A1"].SetStyle(dxfCollection[0]);

            // Guardar el resultado
            workbook.Save("DxfCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Style](../../style/)
* class [DxfCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


