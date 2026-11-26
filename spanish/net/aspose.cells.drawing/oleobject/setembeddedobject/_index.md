---
title: "OleObject.SetEmbeddedObject"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método OleObject. Establece los datos del objeto incrustado."
type: docs
url: /es/net/aspose.cells.drawing/oleobject/setembeddedobject/
---
## SetEmbeddedObject(bool, byte[], string, bool, string) {#setembeddedobject}

Establece los datos del objeto incrustado.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| linkToFile | Booleano | Indica si el objeto está vinculado al archivo. Si es verdadero, se ignora el parámetro objectData. |
| objectData | Byte[] | Los datos del objeto incrustado. |
| sourceFileName | String | El nombre del archivo. |
| displayAsIcon | Booleano | Indica si se muestra el objeto como un ícono. Si es verdadero, los datos de la imagen original serán cubiertos por el ícono. |
| label | String | La etiqueta del ícono. Solo funciona cuando displayAsIcon es verdadero. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un OleObject a la hoja de cálculo
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Preparar parámetros para SetEmbeddedObject
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.xlsx");
                string sourceFileName = "sample.xlsx";
                bool displayAsIcon = false;
                string label = "Excel Document";

                // Llamar a SetEmbeddedObject con los parámetros especificados
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String)");
                
                // Mostrar algunas propiedades para evidenciar el efecto
                Console.WriteLine($"OleObject label: {oleObject.Label}");
                Console.WriteLine($"Display as icon: {oleObject.DisplayAsIcon}");
                Console.WriteLine($"Is linked to file: {oleObject.IsLink}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetEmbeddedObject(bool, byte[], string, bool, string, bool) {#setembeddedobject_1}

Establece los datos del objeto incrustado.

```csharp
public void SetEmbeddedObject(bool linkToFile, byte[] objectData, string sourceFileName, 
    bool displayAsIcon, string label, bool updateIcon)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| linkToFile | Booleano | Indica si el objeto está vinculado al archivo. Si es verdadero, se ignora el parámetro objectData. |
| objectData | Byte[] | Los datos del objeto incrustado. |
| sourceFileName | String | El nombre del archivo. |
| displayAsIcon | Booleano | Indica si se muestra el objeto como un ícono. Si es verdadero, los datos de la imagen original serán cubiertos por el ícono. |
| label | String | La etiqueta del ícono. Solo funciona cuando displayAsIcon es verdadero. |
| updateIcon | Booleano | Indica si el ícono se actualiza automáticamente. |

### Observaciones

Como Aspose puede actualizar todos los íconos de archivos incrustados, es mejor que puedas agregar el ícono correcto con *updateIcon* en false.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class OleObjectMethodSetEmbeddedObjectWithBooleanByteArrayStringBooleanStringBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un OleObject a la hoja de cálculo
            int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
            OleObject oleObject = worksheet.OleObjects[oleObjectIndex];

            try
            {
                // Preparar parámetros para SetEmbeddedObject
                bool linkToFile = false;
                byte[] objectData = File.ReadAllBytes("sample.docx");
                string sourceFileName = "sample.docx";
                bool displayAsIcon = true;
                string label = "Word Document";
                bool updateIcon = true;

                // Llamar a SetEmbeddedObject con los parámetros especificados
                oleObject.SetEmbeddedObject(linkToFile, objectData, sourceFileName, displayAsIcon, label, updateIcon);

                Console.WriteLine("SetEmbeddedObject executed successfully with parameters (Boolean, Byte[], String, Boolean, String, Boolean)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetEmbeddedObject method: {ex.Message}");
            }

            // Guarda el libro de trabajo
            workbook.Save("OleObjectMethodSetEmbeddedObjectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


