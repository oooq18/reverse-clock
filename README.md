# 反方向的钟 · 时光倒计时

打开网站播放《反方向的钟》，音乐从 **1 分 12 秒** 响起；恭喜弹窗带你「听满 100 遍，回到节日前」。
页面实时倒计时，距离最近节假日的天数、时、分、秒，配合反向时钟与频谱动画。

## 在线预览

<https://oooq18.github.io/reverse-clock/>

> 浏览器安全策略：自动播放被拦截时，轻触屏幕即可开始。

## 自定义配置

打开 `index.html`，修改顶部 `CONFIG`：

| 字段 | 说明 |
| --- | --- |
| `audioStartTime` | 音乐开始播放的时间点（秒），默认 `72`（即 1 分 12 秒） |
| `manualHoliday` | 手动指定节日，如 `{ name:'国庆节', date:'2026-10-01' }`；留 `null` 则自动选最近节日 |
| `holidays` | 节假日清单（会自动选择最近的未来节日） |
| `autoplay` | 是否尝试自动播放，`true` / `false` |

## 替换音乐

把新的歌曲转成 `mp3` 放到 `assets/track.mp3`（可选保留 `assets/track.flac` 作为后备源）即可。

## 本地运行

```bash
python3 -m http.server 8765
# 打开 http://localhost:8765/
```
