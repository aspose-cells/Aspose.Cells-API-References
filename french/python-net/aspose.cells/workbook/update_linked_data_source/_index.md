---
title: update_linked_data_source méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 410
url: /fr/python-net/aspose.cells/workbook/update_linked_data_source/
is_root: false
---
##  update_linked_data_source(external_workbooks) {#list}
Si ce classeur contient des liens externes vers d'autres sources de données,
Aspose.Cells tentera de récupérer les dernières données.



```python
def update_linked_data_source(self, external_workbooks):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| external_workbooks | list | Les classeurs externes sont référencés par ce classeur.<br/>S'il est nul, nous ouvrirons directement les fichiers externes liés.<br/> Si ce n'est pas nul,<br/>nous vérifierons d'abord si le lien externe dans le tableau ;<br/> sinon, nous ouvrirons à nouveau les fichiers externes liés.|
###  Remarques

Si la méthode n'est pas appelée avant le calcul des formules,
Aspose.Cells utilisera les informations précédentes (mises en cache dans le fichier) ;
 Veuillez définir CellsHelper.StartupPath,CellsHelper.AltStartPath,CellsHelper.LibraryPath.
Et veuillez définir Workbook.FilePath si ce classeur provient d'un flux,
sinon Aspose.Cells ne pouvait parfois pas obtenir le chemin complet du lien externe.


###  Voir également
* module [aspose.cells](../../)
* classe [Workbook](/cells/fr/python-net/aspose.cells/workbook)
