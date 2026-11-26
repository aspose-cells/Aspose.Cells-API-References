---
title: "Clase IndividualFontConfigs"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.IndividualFontConfigs. Configuraciones de fuentes para cada objeto Workbook"
type: docs
url: /es/net/aspose.cells/individualfontconfigs/
---
## IndividualFontConfigs class

Configuraciones de fuentes para cada objeto [`Workbook`](../workbook/).

```csharp
public class IndividualFontConfigs
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [IndividualFontConfigs](individualfontconfigs/)() | Ctor. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetFontSources](../../aspose.cells/individualfontconfigs/getfontsources/)() | Obtiene una copia del arreglo que contiene la lista de fuentes |
| [GetFontSubstitutes](../../aspose.cells/individualfontconfigs/getfontsubstitutes/)(string) | Devuelve una matriz que contiene nombres de fuentes sustitutas que se usarán si la fuente original no está presente. |
| [SetFontFolder](../../aspose.cells/individualfontconfigs/setfontfolder/)(string, bool) | Establece la carpeta de fuentes |
| [SetFontFolders](../../aspose.cells/individualfontconfigs/setfontfolders/)(string[], bool) | Establece las carpetas de fuentes |
| [SetFontSources](../../aspose.cells/individualfontconfigs/setfontsources/)(FontSourceBase[]) | Establece las fuentes de tipografía. |
| [SetFontSubstitutes](../../aspose.cells/individualfontconfigs/setfontsubstitutes/)(string, string[]) | Establece los nombres de fuentes sustitutas para un nombre de fuente original dado. |

### Ejemplos

```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassIndividualFontConfigsDemo
    {
        public static void Run()
        {
            // Crea directorios temporales para fuentes
            string tempFontFolder1 = Path.Combine(Path.GetTempPath(), "FontFolder1_" + Guid.NewGuid().ToString());
            string tempFontFolder2 = Path.Combine(Path.GetTempPath(), "FontFolder2_" + Guid.NewGuid().ToString());
            Directory.CreateDirectory(tempFontFolder1);
            Directory.CreateDirectory(tempFontFolder2);

            // Crea un archivo CSV de ejemplo
            string csvFilePath = "sample_data.csv";
            File.WriteAllText(csvFilePath, "Name,Age\nJohn,30\nAlice,25", Encoding.UTF8);

            try
            {
                // Inicializa la configuración de fuentes
                IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

                // Establece fuentes sustitutas para Arial
                fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Verdana" });

                // Configura los directorios de fuentes
                fontConfigs.SetFontFolder(tempFontFolder1, false);
                fontConfigs.SetFontFolders(new string[] { tempFontFolder1, tempFontFolder2 }, true);

                // Configura las fuentes
                FontSourceBase[] fontSources = {
                    new FolderFontSource(tempFontFolder1, false),
                    new FolderFontSource(tempFontFolder2, true)
                };
                fontConfigs.SetFontSources(fontSources);

                // Crear opciones de carga de texto con configuraciones de fuente
                TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
                {
                    FontConfigs = fontConfigs
                };

                // Cargar libro de trabajo con opciones configuradas
                using (Workbook workbook = new Workbook(csvFilePath, loadOptions))
                {
                    // Guardar como archivo Excel
                    workbook.Save("output_with_font_config.xlsx");
                }
            }
            finally
            {
                // Limpiar recursos temporales
                if (Directory.Exists(tempFontFolder1)) Directory.Delete(tempFontFolder1, true);
                if (Directory.Exists(tempFontFolder2)) Directory.Delete(tempFontFolder2, true);
                if (File.Exists(csvFilePath)) File.Delete(csvFilePath);
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


