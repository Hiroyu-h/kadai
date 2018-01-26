# 課題１　標本化間隔と空間解像度

標本化間隔を広くすることによる解像度の変化を確認する．
下記はプログラムである．標本化間隔を広くするには原画像を縮小した後画像を拡大する．

clear; % 変数のオールクリア

ORG=imread('C:\Users\lucky\Desktop\neko.png'); % 原画像の入力  
imagesc(ORG); axis image; % 画像の表示  
pause; % 一時停止  

%1/2倍  
IMG = imresize(ORG,0.5); % 画像の縮小  
IMG2 = imresize(IMG,2,'box'); % 画像の拡大  
imagesc(IMG2); axis image; % 画像の表示  
pause; % 一時停止  

%1/4倍  
IMG = imresize(IMG,0.5); % 画像の縮小  
IMG2 = imresize(IMG,4,'box'); % 画像の拡大  
imagesc(IMG2); axis image; % 画像の表示  
pause; % 一時停止  

%1/8倍  
IMG = imresize(IMG,0.5); % 画像の縮小  
IMG2 = imresize(IMG,8,'box'); % 画像の拡大  
imagesc(IMG2); axis image; % 画像の表示  
pause; % 一時停止  

%1/16倍  
IMG = imresize(IMG,0.5); % 画像の縮小  
IMG2 = imresize(IMG,16,'box'); % 画像の拡大  
imagesc(IMG2); axis image; % 画像の表示  
pause; % 一時停止  

%1/32倍  
IMG = imresize(IMG,0.5); % 画像の縮小  
IMG2 = imresize(IMG,32,'box'); % 画像の拡大  
imagesc(IMG2); axis image; % 画像の表示  

このプログラムを実行することで原画像のダウンサンプリングが行われる．  
結果は以下の通りである．  

![Alt text](MATLAB/kadai1/kadai1_1.fig)  図１　原画像  
