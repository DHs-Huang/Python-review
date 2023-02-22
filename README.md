[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/DHs-Huang/Python-code/HEAD?urlpath=tree)
# Python-code
Python重要觀念整理，包含物件導向、裝飾器等議題，方便複習以及銜接後續模組應用  
也同時探討進階議題，包含各個Python版本更新的重要內容以及各種Pythonic的技巧等內容
## 觀念整理
### [物件導向 (Object Oriented Programming)觀念整理](OOP/OOP_concepts_Python.ipynb)
* 繼承 (inheritance)
* 封裝 (encapsulation)  
  [OOP property uses for encapsulation](OOP/OOP_property.ipynb)
* 多型 (polymorphism)
* [Class methods介紹](OOP/OPP_class_methods.ipynb)

### [裝飾器 (Decorator)觀念整理](Decorator.ipynb)

## 進階議題 
### [Python版本更新](Advanced-issues/Add_new_features.ipynb)
* Python 3.5
  * 矩陣乘法專用的運算符@
  * 解構列表，\**解構字典
  * `typing model`用於註解參數與回傳型態 (此文檔於Python 3.8說明)
* Python 3.6
  * f-string (後續亦增加其他用法)
  * async 和 await的協同生成器 (後續版本亦有更新)
  * secrets module用於password等管理
* Python 3.7
  * 內建breakpoint
  * 類型和註解
  * dictionary保持插入順序
  * `dataclass`
* Python 3.8
  * :=海象賦值 → (variable_name := expression)，用於if, while等協助減少呼叫asssignment的次數以及順暢邏輯
  * 詳細定義位置參數以及關鍵字參數的區隔
  * fstring可用=直接表示變數
  * typing模組的改進:Python是動態類型語言，但可以通過typing模組添加類型提示，以便協力廠商工具驗證Python代碼。Python 3.8給typing添加了一些新元素，因此它能夠支援更健壯的檢查：
    * final修飾器和Final類型標注表明，被修飾或被標注的物件在任何時候都不應該被重寫、繼承，也不能被重新賦值。
    * Literal類型將運算式限定為特定的值或值的列表（不一定是同一個類型的值）。
    * TypedDict可以用來創建字典，其特定鍵的值被限制在一個或多個類型上。注意這些限制僅用於編譯時確定值的合法性，而不能在運行時進行限制。
* Python 3.9
  * 字典更新和合併：|運算符用於合併字典，|= 運算符用於更新字典
  * 最小公倍數 math.LCM* Python 3.9 將兩個新函數添加到 str 對象：
  * 第一個函數用於刪除前綴：str.removeprefix(prefix); 第二個函數用於刪除後綴：str.removesuffix(suffix)
  * 對異步編程（asyncio）和多進程庫進行了優化
  * 增加randbytes
截至(2023/02/04)anaconda尚未更新
* Python 3.10
  * switch case判斷式
  * 顯示詳細的錯誤資訊
  * Union可以用其他運算子代替
  * 嚴謹的zip
  * with語法可以一次開多個檔案
* Python 3.11
  * 比上一个版本快60% (The most important one)
  * 改進的錯誤提示
  * self也可以被類別提示 (from \_\_future\_\_ import annotations)
  * Typedict in typing可建立非必要元素

### Pythonic
* [Underscore多種用法](Advanced-issues/Underline_illustration.ipynb)