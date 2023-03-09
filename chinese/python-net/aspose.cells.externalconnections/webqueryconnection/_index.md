---
title: WebQueryConnection类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 70
url: /zh/python-net/aspose.cells.externalconnections/webqueryconnection/
is_root: false
---
## WebQueryConnection类
 Web 查询将从 HTML 表中检索数据，
并且还可以提供 HTTP“获取”参数，由 Web 服务器在生成 HTML 时进行处理
包括参数和参数元素。



**继承：** [WebQueryConnection](/cells/python-net/aspose.cells.externalconnections/webqueryconnection) → 
[ExternalConnection](/cells/zh/python-net/aspose.cells.externalconnections/externalconnection)



WebQueryConnection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [id](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/id) |获取连接的 ID。|
| [power_query_formula](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/power_query_formula) |获取幂查询公式的定义。|
| [type](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/type) |获取或设置外部连接数据源类型。|
| [source_file](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/source_file) |当外部数据源是基于文件的时使用。<br/> source 失败，电子表格应用程序尝试直接连接到该文件。<br/>以 URI 或系统特定的文件路径表示法表示。|
| [sso_id](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/sso_id) |用于中间体之间身份验证的单点登录 (SSO) 标识符<br/>spreadsheetML 服务器和外部数据源。|
| [save_password](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/save_password) |如果要将密码保存为连接字符串的一部分，则为 True；否则为 False。|
| [save_data](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/save_data) |如果要保存通过连接获取的用于填充表的外部数据，则为真<br/>与工作簿一起；否则，错误。|
| [refresh_on_load](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_on_load) |如果在打开文件时应刷新此连接，则为真；否则为真。|
| [reconnection_method_type](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method_type) |指定当连接失败时电子表格应用程序应该做什么。<br/>默认值为 ReConnectionMethodType.Required。|
| [reconnection_method](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/reconnection_method) |指定当连接失败时电子表格应用程序应该做什么。<br/>默认值为 ReConnectionMethodType.Required。|
| [only_use_connection_file](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/only_use_connection_file) |指示电子表格应用程序是否应始终且仅使用<br/>odcFile 属性指示的外部连接文件中的连接信息<br/>当连接刷新时。如果为 false，则电子表格应用程序<br/>应遵循 reconnectionMethod 属性指示的过程|
| [odc_file](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/odc_file) |指定此连接来自的外部连接文件的完整路径<br/>如果在尝试刷新数据时连接失败，并且 reconnectionMethod=1，<br/>然后电子表格应用程序将使用来自外部连接文件的信息重试<br/>而不是工作簿中嵌入的连接对象。|
| [is_new](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/is_new) |如果连接不是第一次刷新，则为 True；否则为 false。<br/>当用户在查询完成返回之前保存文件时，就会发生这种状态。|
| [name](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/name) |指定连接的名称。|
| [keep_alive](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/keep_alive) |当电子表格应用程序应努力保持连接时为真<br/>打开。如果为 false，应用程序应在检索到<br/>信息。|
| [refresh_internal](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/refresh_internal) |指定连接自动刷新之间的分钟数。|
| [connection_id](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/connection_id) |指定此连接的唯一标识符。|
| [connection_description](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/connection_description) |指定此连接的用户描述|
| [is_deleted](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/is_deleted) |指示关联的工作簿连接是否已被删除。如果<br/>否则，假的。|
| [credentials_method_type](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/credentials_method_type) |指定建立（或重新建立）连接时要使用的身份验证方法。|
| [credentials](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/credentials) |指定建立（或重新建立）连接时要使用的身份验证方法。|
| [background_refresh](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/background_refresh) |指示是否可以在后台（异步）刷新连接。<br/>如果连接的首选用法是在后台异步刷新，则为真；<br/>如果连接的首选用法是在前台同步刷新，则为 false。|
| [parameters](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/parameters) |为 ODBC 或 Web 查询获取 [ConnectionParameterCollection](/cells/zh/python-net/aspose.cells.externalconnections/connectionparametercollection)。|
| [is_xml](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml) |如果 Web 查询源是 XML（相对于 HTML），则为 true，否则为 false。|
| [is_xl97](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl97) |此标志的存在是为了向后兼容旧的现有电子表格文件，并已设置<br/>如果此 Web 查询是在 Microsoft Excel 97 中创建的，则为真。<br/>这是一个可以忽略的可选属性。|
| [is_xl2000](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/is_xl2000) |此标志的存在是为了向后兼容旧的现有电子表格文件，并已设置<br/>如果此 Web 查询在更新或等于的电子表格应用程序中刷新，则为真<br/>至 Microsoft Excel 2000。<br/>这是一个可以忽略的可选属性。|
| [url](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/url) |用于刷新外部数据的 URL。|
| [is_text_dates](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/is_text_dates) |指示日期是否应作为文本而不是日期导入到工作表中的单元格中的标志。|
| [is_xml_source_data](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/is_xml_source_data) |指示应该导入 XML 源数据而不是 HTML 表本身的标志。|
| [post](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/post) |返回或设置用于将数据输入到 Web 服务器的 post 方法的字符串<br/>从网络查询返回数据。|
| [is_parse_pre](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/is_parse_pre) |标志表示网页中 HTML PRE 标签中包含的数据是否是<br/>将页面导入查询表时解析为列。|
| [is_html_tables](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/is_html_tables) |指示 Web 查询是否仅适用于 HTML 表的标志。|
| [html_format](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/html_format) |将 Web 查询数据引入时如何处理来自 HTML 源的格式<br/>工作表。当 sourceData 为 True 时相关。|
| [is_same_settings](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/is_same_settings) |指示是否解析具有相同宽度设置的 PRE 块内的所有表的标志<br/>作为第一行。|
| [edit_web_page](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/edit_web_page) |显示网络查询数据的面向用户的网页的 URL。<br/>在 sourceData="true" 和 url 已被重定向以引用 XML 文件的情况下。<br/>然后可以在 UI 中显示面向用户的页面，并且可以检索 XML 数据<br/>在幕后。|
| [edit_page](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/edit_page) |显示网络查询数据的面向用户的网页的 URL。<br/>在 sourceData="true" 和 url 已被重定向以引用 XML 文件的情况下。<br/>然后可以在 UI 中显示面向用户的页面，并且可以检索 XML 数据<br/>在幕后。|
| [is_consecutive](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection/is_consecutive) |指示是否应将连续的定界符仅视为一个定界符的标志。|



### 也可以看看
* 模块 [aspose.cells.externalconnections](..)
* 类 [ConnectionParameterCollection](/cells/zh/python-net/aspose.cells.externalconnections/connectionparametercollection)
* 类 [ExternalConnection](/cells/zh/python-net/aspose.cells.externalconnections/externalconnection)
* 类 [WebQueryConnection](/cells/zh/python-net/aspose.cells.externalconnections/webqueryconnection)
