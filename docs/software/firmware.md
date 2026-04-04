# 7. 修改與燒錄 Openclaw 韌體

有時候我們需要修改小龍蝦機的預設參數，就不想從頭開始編寫程式，可以使用官方發布的編譯工具，直接修改並燒錄。

這種方法只適用於修改量較小，且對 C++ 與硬體架構較為熟悉的開發人員使用。

!!! warning "注意"
    通用韌體必須在 Windows 下，使用 `Openclaw_Flash_Tool` 進行打包、解包，否則打包出來的韌體無法正常使用。請務必確認主板的 USB 驅動程式已正確安裝。

## 7.1. 獲取燒錄工具與解壓縮

訪問我們的 GitHub Release 頁面，獲取 `Openclaw_Flash_Tool_v1.0.zip`，將該檔案解壓縮到你的電腦中。

使用終端機（或命令提示字元）進入該目錄並執行解壓縮：

```bash linenums="1"
# 進入下載目錄並解壓
cd Downloads/
unzip Openclaw_Flash_Tool_v1.0.zip