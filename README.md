https://fx63065.pythonanywhere.com/findfoxfox/
這是期末專題連結

!!!內容說明!!!

1.內容(有主頁以及分頁)

主頁:最上層是 狐狸百科(主題)和右上角的一些說明(網站介紹 顯示全部 回饋)
網站介紹中有說明網站的基本用法 至於回饋的部分 後端正在學習中 因此還沒此功能
主頁:搜尋欄有提示字的功能 打好字後 按Enter或是 確認 按鈕都可以查詢
主頁:底下的照片點下後可以直接跳轉到新的頁面(對應種類的狐狸)

分頁:左側是對應種類的狐狸名稱及相關資料(分類 外觀 習性 交流 食物)點下後右側的資料會跳轉到相應的地方
分頁:右側是此狐狸相關的資料

2.程式/邏輯(html css javascript)
這個網頁目前只有用到前端3要素

html:主要的文本內容
css:修飾html文本內容(排版 顏色...)
另外此網站有設置不同視窗大小會自動調整文本(響應式網頁)
javascript:增加互動性 其中搜尋欄的提示字功能就是javascript做的

3.遇到的問題:
主要會是javascript
因為在此專題前我根本不會javascript
是為了做出文字輸入框相關的功能才開始學的

像是如何取用html中的標籤啦:
const box=document.querySelector(".box");
將按鈕視為Enter鍵啦:
if (button){
    button.addEventListener("click",function(){
        const fakekey=new KeyboardEvent("keyup",{
            key:'Enter',
            code:'Enter',
            keyCode:13,
            which:13,
            bubbles:true,
            cancelable:true
        });
        box.dispatchEvent(fakekey);
    });
}
判斷使用者按了什麼案件啦:
box.addEventListener("keyup",function(f){(這段太長了 只抓前面的說明)
等等...
反正從頭開始學js真是一大挑戰
