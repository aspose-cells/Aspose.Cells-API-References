---
title: "Clase SensitivityLabel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Metas.SensitivityLabel. Representa la etiqueta de sensibilidad"
type: docs
url: /es/net/aspose.cells.metas/sensitivitylabel/
---
## SensitivityLabel class

Representa la etiqueta de sensibilidad.

```csharp
public class SensitivityLabel
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AssignmentType](../../aspose.cells.metas/sensitivitylabel/assignmenttype/) { get; set; } | Obtiene y establece el método de asignación para la etiqueta de sensibilidad. |
| [ContentMarkType](../../aspose.cells.metas/sensitivitylabel/contentmarktype/) { get; set; } | Obtiene y establece los tipos de marcado de contenido que deben aplicarse a un archivo. |
| [Id](../../aspose.cells.metas/sensitivitylabel/id/) { get; set; } | Obtiene y establece el id de la etiqueta de sensibilidad. |
| [IsEnabled](../../aspose.cells.metas/sensitivitylabel/isenabled/) { get; set; } | Indica si la etiqueta de sensibilidad está habilitada |
| [IsRemoved](../../aspose.cells.metas/sensitivitylabel/isremoved/) { get; set; } | Indica si la etiqueta de sensibilidad fue eliminada. |
| [SiteId](../../aspose.cells.metas/sensitivitylabel/siteid/) { get; set; } | Representa el identificador del sitio de Azure Active Directory (Azure AD) correspondiente a la política de etiqueta de sensibilidad que describe la etiqueta de sensibilidad. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Metas;
    using System;

    public class MetasClassSensitivityLabelDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            
            try
            {
                // Crear una instancia de la clase SensitivityLabel usando reflexión
                SensitivityLabel label = (SensitivityLabel)Activator.CreateInstance(typeof(SensitivityLabel));
                
                // Establecer propiedades básicas
                label.Id = "CONFIDENTIAL_001";
                label.IsEnabled = true;
                label.AssignmentType = SensitivityLabelAssignmentType.Standard;
                label.ContentMarkType = SensitivityLabelMarkType.None;
                
                // Mostrar valores de propiedades
                Console.WriteLine($"Sensitivity Label Created:");
                Console.WriteLine($"ID: {label.Id}");
                Console.WriteLine($"Enabled: {label.IsEnabled}");
                Console.WriteLine($"Assignment Type: {label.AssignmentType}");
                Console.WriteLine($"Content Mark Type: {label.ContentMarkType}");
                
                // Guarda el libro de trabajo
                workbook.Save("SensitivityLabelDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with SensitivityLabel: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Metas](../../aspose.cells.metas/)
* assembly [Aspose.Cells](../../)


