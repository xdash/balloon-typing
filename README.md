# balloon-typing

气球打字 · 打字消除网页游戏。单文件 HTML（`index.html`），零依赖零构建，手机键盘可用。

- 字母写在一个个气球上，气球从底部不断升起，按键盘上对应的字母即戳爆该气球
- 连续戳爆有连击加成（×N），得分随连击翻倍
- 打错字母掉连击；漏掉 5 个气球游戏结束
- 开局铺 4 个错落气球，之后按 1.05s → 0.42s 逐渐加速生成；气球也随局时变大变小
- 得分/最高分/静音偏好存 localStorage
- 音效用 WebAudio 合成（pop / 漏气 / 打错），零外部音频文件
- 漏掉的气球计入「漏气」并显示剩余次数；结算页显示戳爆数、漏掉数、戳到最高的高度（px）

线上地址：https://xdash.me/balloon-typing/ （GitHub Pages，独立 repo `xdash/balloon-typing`，push main → 自动发布）

## 本地预览

```bash
python3 -m http.server 8000
# 打开 http://localhost:8000
```