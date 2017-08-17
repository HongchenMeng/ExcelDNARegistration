Excel-DNA Registration Helper
===============================
Excel-DNA注册助手
=============================
原作者：Govert <br>
作者github：https://github.com/Excel-DNA
______________________________________

_This library implements helper functions to assist and modify the Excel-DNA function registration, by applying various transformations before the functions are registered.<br>
_这个库实现了帮助函数，以帮助和修改Excel DNA函数注册，通过在函数注册之前应用各种转换。<br>

_The following transformations have been implemented:<br>
_实现了以下转换：<br>

_Generation of wrapper functions for:<br>
_包装函数的生成：<br>

- Functions returning Task<T> or IObservable<T> as asynchronous or RTD-based functions (including F# Async<T> functions)<br>
- Optional parameters (with default values), 'params' parameters and Nullable<T> parameters<br>
- Range parameters in Visual Basic functions<br>
- 异步函数或RTD函数返回Task<T> or IObservable<T> （包括F# Async<T>函数）<br>
- 可选参数（默认值），params参数和Nullable<T>参数<br>
- VisualBasic函数中的范围参数<br>

_Examples of general function transformations:<br>
_一般函数变换的例子：<br>

- Logging / Caching / Timing handlers<br>
- Suppress in Function Arguments dialog<br>
-记录/缓存/定时处理程序<br>
-在函数参数对话框中禁止<br>

_If you've previously used the CustomRegistration library, note that I've renamed and rearranged the project source, and renamed the output assembly from ExcelDna.CustomRegistration to ExcelDna.Registration. The last state of the project before the large-scale rearrangement is marked by the git tag **CustomRegistration_Before_Rename**, and can be retrieved from the release tab on GitHub.<br>
_如果你以前使用的customregistration类库，注意，我改名和重新安排的项目源，并改名为输出组件从exceldna.customregistration到exceldna.registration。最后状态的项目之前，大规模的重组的特点是git tag * customregistration_before_rename **，并且可以从GitHub上发布标签检索。<br>

### _Registration [Error] Repeated function name..._
_If you receive this error when opening your Excel addin, you need to add `ExplicitRegistration='true'` to the `<ExternalLibrary Path='MyAddin.dll'...` command in your .dna file_.
### _Registration [Error] Repeated function name..._
_如果您收到此错误打开Excel插件时，你需要加` explicitregistration =真实的`的` < externallibrary路径= 'myaddin .dll”…`命令在你的DNA file_。
