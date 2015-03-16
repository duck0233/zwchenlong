#Linux下無法顯示字型

# Linux用家請注意 #

最近發現Mono於Ubuntu 9.10無法取得XIM輸入，變相於本程式無法輸入中文。網上討論發現Fedora Linux亦有同樣情況。

另，如是使用Intel Graphic Chipset，於Ubuntu 9.10所提供的Intel driver (server-xorg-video-intel (2:2.9.0-1ubuntu2))並無法顯示程式字型。以下為解決方法：

  1. add-apt-repository ppa:xorg-edgers/ppa
  1. apt-get update
  1. apt-get upgrade

又，測試時發現Linux下需安裝[「新細明體」](http://mingliu.myweb.hinet.net/MingLiu/MingLiU.zip)才能正常顯示中文。

安裝方式：

  1. 在/usr/share/fonts/truetype下開一個資料夾，例如windows-fonts；
  1. 下載並解壓細明體，並把MingLiU.ttc丟進去；
  1. 執行fc-cache -f -v字型快取更新即可。