# RimeInputMethodEngine Rime輸入法備份文件

## 說明
這是我在Linux Ubuntu 中使用 Fcitx5-rime輸入法中安裝小鶴雙拼+注音的備份檔，
只要安裝此備份檔即可使用小鶴雙拼+注音

>在此附上[原輸入法Github](https://github.com/JeffChien/rime-flypyquick5)


## 安裝方式
>參考[巴哈教學安裝](https://home.gamer.com.tw/artwork.php?sn=5577703)

在Ubuntu中打開終端機
- 安裝 fcitx5 輸入框架
```bash
sudo apt install fcitx5
```
- 安裝 fcitx5 用的 RIME
```bash
sudo apt install fcitx5-rime
```
- 下載東風破（plum）

```bash
git clone https://github.com/rime/plum.git && cd plum
```
- 用東風破下載注音輸入法
```bash
rime_frontend=fcitx5-rime bash rime-install bopomofo terra-pinyin
```
- 在Ubuntu　應用程式中 找到fcitx5Configuration並打開
- 在input Method / Available input Method 找到rime 並add to Current input Method 然後Apply
- 重開機有出現鍵盤圖示即可用ctrl + 空白鍵選擇輸入法
- 如果沒出現的話在終端機輸入並重開機
```bash
im-config -n fcitx5
```
- 如果還是沒有的話終端機輸入並重開機
```bash
mkdir -p ~/.config/autostart && cp /usr/share/applications/org.fcitx.Fcitx5.desktop ~/.config/autostart
```
- 接下來到```bash ~/.local/share/fcitx5/rime/ ```資料夾中將此Github檔案全部複製進去
- 並重新啟動Fictx5 用Ctrl + 空白鍵選到中州韻
- 按F4 選擇小鶴雙拼+速成 










