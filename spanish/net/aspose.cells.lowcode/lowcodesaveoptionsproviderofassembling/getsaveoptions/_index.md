---
title: "LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "LowCodeSaveOptionsProviderOfAssembling method. Obtiene las opciones de guardado de las que se extraen los ajustes de salida para la parte dividida actual"
type: docs
url: /es/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/
---
## LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions method

Obtiene las opciones de guardado de las que se extraen los ajustes de salida para la parte dividida actual.

```csharp
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingMethodGetSaveOptionsWithSplitPartInfoDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].Value = "Sample Data for Split";

            try
            {
                // Crear una instancia de LowCodeSaveOptionsProviderOfAssembling
                var provider = new LowCodeSaveOptionsProviderOfAssembling
                {
                    PathHeader = "Output/",
                    PathTail = ".xlsx",
                    UseSheetName = true,
                    SheetPrefix = "Sheet_",
                    SplitPartPrefix = "Part_",
                    SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
                };

                // Crea una instancia de SplitPartInfo usando reflexión ya que el constructor no es accesible
                var splitPartInfo = (SplitPartInfo)Activator.CreateInstance(typeof(SplitPartInfo), nonPublic: true);

                // Llama a GetSaveOptions con el parámetro SplitPartInfo
                LowCodeSaveOptions saveOptions = provider.GetSaveOptions(splitPartInfo);

                Console.WriteLine("SaveOptions created successfully");
                Console.WriteLine($"Output format: {saveOptions.SaveFormat}");

                // Guarda el libro de trabajo (en un uso real esto usaría las opciones de guardado generadas)
                workbook.Save("GetSaveOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in GetSaveOptions demo: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


