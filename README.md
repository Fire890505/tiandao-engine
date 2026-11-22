# 天道棋盤 引擎（聊天版用）

只用 Python 標準函式庫（3.11 以上）。原本的程式整套照跑，只有「模型寫字」那一步交給聊天裡的 Claude。

```
git clone --depth 1 https://github.com/Fire890505/tiandao-engine.git
cd tiandao-engine && unzip -q -o tiandao_engine.zip
python -m tiandao.chat new 名字 性別 [時代]   # 開世界
python -m tiandao.chat turn "玩家這句"         # 一回合
python -m tiandao.chat answer                  # 寫好 棋盤/ai_answer.json 後接著跑
python -m tiandao.chat write                   # 寫背景內容（物品、傳說、怪談、事端）
python -m tiandao.chat state                   # 角色卡
python -m tiandao.chat save 檔名 / load 檔名   # 存檔、讀檔
```

錢：程式裡一律記凡人錢；給玩家和說書看的照時代換算（古代 ×20 文、現代 ×600 元、未來 ×100 點），玩家說的錢換回凡人錢。只在 chat.py，網頁版不變。

更新：重新打包 tiandao_engine.zip（tiandao/ 和 rules/）覆蓋同名檔。
