　　辰龍使用的是Linux。要寫斗數排盤程式，當然憂先能在Linux下使用。

　　在初考慮，能否實作出安星法則只是次要，更為重要是如何將斗數生盤顯示出來。有想過用Linux原生Gtk+為開發環境，然因在顯示畫面方便文檔稀少，對不諳程式如我，很難入手。況且Gtk+基於C語言，實不太方便。

　　較為易用的語言有Java，其好處還有可誇平台使用。已有朋友送贈用Java寫成的斗數排盤程式，但總覺得其字體顯示十分怪異。

　　之前曾有看過一些.Net Framework的資料，發現C＃在很多地方「參考」了Java的易用性，且由微軟原生支援，應該可用。

　　Linux下有一Mono Project，免費提供了.Net Framework的編譯環境，當中提供寫視窗界面必備的WinForm Namespace，且有頗完善的開發環境MonoDevelop。

　　手上剛好有Charles Petzold寫的Programming Microsoft Windows with C#，詳細介紹了如何利用C#寫出視窗程式。於是便選定C#，利用Linux下的MonoDevelop整合開發環境進行寫作。