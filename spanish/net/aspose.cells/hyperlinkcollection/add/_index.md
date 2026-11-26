---
title: "HyperlinkCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método HyperlinkCollection. Añade un hipervínculo a una celda especificada o a un rango de celdas"
type: docs
url: /es/net/aspose.cells/hyperlinkcollection/add/
---
## Add(int, int, int, int, string) {#add}

Agrega un hipervínculo a una celda especificada o a un rango de celdas.

```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| firstRow | Int32 | Primera fila del rango de hipervínculo. |
| firstColumn | Int32 | Primera columna del rango de hipervínculo. |
| totalRows | Int32 | Número de filas en este rango de hipervínculo. |
| totalColumns | Int32 | Número de columnas de este rango de hipervínculo. |
| address | String | Dirección del hipervínculo. |

### Valor de retorno

[`Hyperlink`](../../hyperlink/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithInt32Int32Int32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añadir hipervínculo usando coordenadas de fila/columna y dimensiones
            worksheet.Hyperlinks.Add(0, 0, 1, 1, "http://www.aspose.com");
            worksheet.Hyperlinks.Add(1, 0, 1, 1, "c:\\book1.xls");
            
            workbook.Save("HyperlinkDemo.xlsx");
        }
    }
}
```

### Ver también

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, int, int, string) {#add_1}

Agrega un hipervínculo a una celda especificada o a un rango de celdas.

```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | Nombre de la celda. |
| totalRows | Int32 | Número de filas en este rango de hipervínculo. |
| totalColumns | Int32 | Número de columnas de este rango de hipervínculo. |
| address | String | Dirección del hipervínculo. |

### Valor de retorno

[`Hyperlink`](../../hyperlink/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringInt32Int32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Añadir hipervínculo a la celda A1 con la dirección "www.aspose.com"
            hyperlinks.Add("A1", 1, 1, "www.aspose.com");
            
            // Mostrar la dirección del hipervínculo
            Console.WriteLine("Hyperlink Address: " + worksheet.Cells["A1"].StringValue);
            
            // Cambiar el texto de visualización
            worksheet.Cells["A1"].PutValue("Click Here");
            Console.WriteLine("Display Text: " + hyperlinks[0].TextToDisplay);
            
            workbook.Save("HyperlinkExample.xlsx");
        }
    }
}
```

### Ver también

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string, string, string, string, string) {#add_2}

Agrega un hipervínculo a una celda especificada o a un rango de celdas.

```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay, 
    string screenTip)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| startCellName | String | La celda superior izquierda del rango. |
| endCellName | String | La celda inferior derecha del rango. |
| address | String | Dirección del hipervínculo. |
| textToDisplay | String | El texto que se mostrará para el hipervínculo especificado. |
| screenTip | String | El texto screenTip para el hipervínculo especificado. |

### Valor de retorno

[`Hyperlink`](../../hyperlink/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HyperlinkCollectionMethodAddWithStringStringStringStringStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            HyperlinkCollection hyperlinks = worksheet.Hyperlinks;

            // Demostrar el método Add con parámetros (String, String, String, String, String)
            hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");

            workbook.Save("HyperlinkCollectionExample.xlsx");
        }
    }
}
```

### Ver también

* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


