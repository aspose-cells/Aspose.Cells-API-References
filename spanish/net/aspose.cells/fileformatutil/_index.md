---
title: "Clase FileFormatUtil"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.FileFormatUtil. Proporciona métodos utilitarios para convertir enumeraciones de formato de archivo a cadenas o extensiones de archivo y viceversa"
type: docs
url: /es/net/aspose.cells/fileformatutil/
---
## FileFormatUtil class

Proporciona métodos de utilidad para convertir enumeraciones de formato de archivo a cadenas o extensiones de archivo y viceversa.

```csharp
public class FileFormatUtil
```

## Métodos

| Nombre | Descripción |
| --- | --- |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat)(Stream) | Detecta y devuelve la información sobre un formato de un Excel almacenado en un flujo. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_2)(string) | Detecta y devuelve la información sobre un formato de un Excel almacenado en un archivo. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_1)(Stream, string) | Detecta y devuelve la información sobre un formato de un Excel almacenado en un flujo. |
| static [DetectFileFormat](../../aspose.cells/fileformatutil/detectfileformat/#detectfileformat_3)(string, string) | Detecta y devuelve la información sobre un formato de un Excel almacenado en un archivo. |
| static [ExtensionToSaveFormat](../../aspose.cells/fileformatutil/extensiontosaveformat/)(string) | Convierte la extensión del nombre de archivo en un valor SaveFormat. |
| static [FileFormatToSaveFormat](../../aspose.cells/fileformatutil/fileformattosaveformat/)(FileFormatType) | Convirtiendo el formato de archivo a formato de guardado. |
| static [IsTemplateFormat](../../aspose.cells/fileformatutil/istemplateformat/)(string) | Devuelve true si la extensión es .xlt, .xltX, .xltm, .ots. |
| static [LoadFormatToExtension](../../aspose.cells/fileformatutil/loadformattoextension/)(LoadFormat) | Convierte un valor enumerado de formato de carga en una extensión de archivo. |
| static [LoadFormatToSaveFormat](../../aspose.cells/fileformatutil/loadformattosaveformat/)(LoadFormat) | Convierte un valor LoadFormat a un valor SaveFormat si es posible. |
| static [SaveFormatToExtension](../../aspose.cells/fileformatutil/saveformattoextension/)(SaveFormat) | Convierte un valor enumerado de formato de guardado en una extensión de archivo. |
| static [SaveFormatToLoadFormat](../../aspose.cells/fileformatutil/saveformattoloadformat/)(SaveFormat) | Convierte un valor SaveFormat a un valor LoadFormat si es posible. |
| static [VerifyPassword](../../aspose.cells/fileformatutil/verifypassword/)(Stream, string) | Detecta y devuelve la información sobre un formato de un Excel almacenado en un flujo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassFileFormatUtilDemo
    {
        public static void Run()
        {
            string filePath = "example.xlt";
            
            // Detectar formato de archivo
            FileFormatInfo info = FileFormatUtil.DetectFileFormat(filePath);
            Console.WriteLine("Detected file format: " + info.FileFormatType);
            
            // Verificar formato de archivo con Workbook
            Workbook workbook = new Workbook(filePath);
            Console.WriteLine("Workbook file format: " + workbook.FileFormat);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


