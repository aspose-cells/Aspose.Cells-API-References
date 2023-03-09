---
title: LoadFilter classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1010
url: /fr/python-net/aspose.cells/loadfilter/
is_root: false
---
##  LoadFilter classe
Représente le filtre qui fournit des options pour le chargement des données lors du chargement du classeur à partir du modèle.



Le type LoadFilter expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [LoadFilter()](/cells/fr/python-net/aspose.cells/loadfilter/__init__/#) | Construit un LoadFilter avec les options de filtre par défaut LoadDataFilterOptions.All.|
| [LoadFilter(opts)](/cells/fr/python-net/aspose.cells/loadfilter/__init__/#LoadDataFilterOptions) | Construit un LoadFilter avec des options de filtre données.|


###  Propriétés
| Propriété| Description|
| :- | :- |
| [load_data_filter_options](/cells/fr/python-net/aspose.cells/loadfilter/load_data_filter_options) | Les options de filtre pour indiquer quelles données doivent être chargées.|
| [sheets_in_loading_order](/cells/fr/python-net/aspose.cells/loadfilter/sheets_in_loading_order) | Spécifie les feuilles (indices) et l'ordre à charger.<br/>La valeur par défaut est null, ce qui signifie qu'il faut charger toutes les feuilles dans l'ordre par défaut dans le fichier modèle.<br/> S'il n'est pas nul et que l'index de certaines feuilles n'est pas dans le tableau renvoyé, la feuille ne sera pas chargée.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [start_sheet(sheet)](/cells/fr/python-net/aspose.cells/loadfilter/start_sheet/#Worksheet) | Prépare les options de filtre avant de charger la feuille de calcul donnée.<br/>L'implémentation de LoadFilter par l'utilisateur peut modifier les LoadDataFilterOptions ici<br/> pour indiquer comment charger les données pour cette feuille de calcul.|



###  Remarques

L'utilisateur peut spécifier les options de filtre ou implémenter son propre LoadFilter pour spécifier comment charger les données.

###  Voir également
* module [aspose.cells](..)
