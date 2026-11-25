# guitar-media-2

个人网站 [fanyu-meng.github.io](https://fanyu-meng.github.io/) 的视频存档，由网站仓库的
`scripts/archive-videos.py` 生成。开启了 GitHub Pages（`main` 分支、根目录），
文件地址是 `https://fanyu-meng.github.io/guitar-media-2/<视频ID>/…`。

- `<视频ID>/video.mp4`：H.264 + AAC，平台上的最高画质，未重新编码。
- `<视频ID>/index.m3u8` 和 `seg-NNNN.ts`：超过 95 MB 的视频切成的 HLS 分段，同样未重新编码。
- `manifest.json`：每条视频的路径、大小、分辨率、时长和来源。网站据此生成 `public/content/video-media.json`。

本仓库控制在约 800 MB 以内（Pages 每个站点上限约 1 GB）。装满后新视频放进下一个仓库。
