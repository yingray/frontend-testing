# Introduction

本篇文章介紹單元測試應用於前端框架React-Redux。

## What We Test For?

我們前端工程師對於Web的測試關注於：

* 輸入的驗證
* 資料的轉變
 
常見的例子如：

1. 模擬操作的事件
*  程式回應的事件
*  程式的渲染
*  不同瀏覽器的測試
*  更新版本後的測試
*  Continuous Integration Systems

> In addition to unit testing (input validation, data transformations, etc):
>
1. Test user events
2. Test response to those events
3. Make sure the right things render at the right time
4. Run tests in different browsers
5. Re-run tests on file change
6. Work with continuous integration systems like Travis https://travis-ci.org/

> Heidi

## 方法

軟體開發中的測試階段依序分為**單元**、**整合**、**系統**、**驗收**，前端開發目前主分為**單元**、**整合**、**端對端**測試。

### 單元測試

單元通常為程式中的最小單位(function)，隔離外層控制進行測試，去除外部操作變因、真實物件執行時間等。

### 端對端測試

E2E測試(End-to-End Testing)為user和app之間的互動來進行測試，所以通常會從user操作的角度去撰寫程式。

### Unit Test vs End-to-End Test

Test                       | Unit                                   | E2E                                 
-------------------------- | -------------------------------------- | ----------------------------------
Testing component          | Single function                        | Entire application
Failed, what's conclusion? | Exact function in exact parameters set | Could be any component related
Coupling?                  | JS implementation                      | html
Who can write the test     | RD                                     | Anyone
Maintenance                | Low                                    | High
Execution cost             | The function and related object        | Entire application


--








