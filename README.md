# 财神视频工作流包 · 站点说明

本站是「财神视频工作流包」（$19 一次性买断）的 GitHub Pages 站：首页、定价、llms.txt、工作流总览、用途页、案例复刻页。

**当前状态：方法已定。** 4 个核心工作流的方法已定，ComfyUI .json 图文件待 GPU 验证；逆向组合方法、Pavo 单人定妆镜头、EP1 v6 已公开案例、提示词库、工具脚本已在包里。不许对外宣称 ComfyUI .json 图文件已经做完、已经发布。购买链接待上架（Gumroad）；域名与 GitHub 仓库已定：域名 https://gmq20100723-sudo.github.io/；GitHub 仓库 https://github.com/gmq20100723-sudo/gmq20100723-sudo.github.io。

## 文件地图

- `index.md` — 首页
- `pricing/index.md` — 定价页（人可读）；`pricing.md` — 定价机器可读版（与定价页同源）
- `llms.txt` — 给 AI 爬虫读的产品说明（照 CreativeClaw 结构）
- `workflows/index.md` — 工作流总览；`workflows.md` — 工作流机器可读版
- `workflows/*/index.md` — 4 个核心工作流详情页（方法已定，ComfyUI .json 图文件待 GPU 验证）
- `workflows/reverse-prompt/for-2d-drama/index.md` — 工作流 × 用途组合页（已填入逆向改核 + 锁脸做法）
- `use-cases/` — 用途着陆页（2.5D 短片、锁脸短片、播报开篇）
- `alternatives/` — 模型替代页
- `benchmarks/` — 实测对比页
- `examples/` — 案例复刻页（EP1 v6 已公开案例 + 案例库与方法/模板笔记，只列文件名与目录原文结论）
- `tutorials/index.md` — 16 篇教程索引（标题已定，正文待填）
- `cost-calculator/index.md` — 成本计算器页
- `help/index.md` — 帮助页
- `.well-known/product.json` — 产品卡片（机器可读）
- `_config.yml` — Jekyll 配置（域名、仓库链接已填；Gumroad 购买链接待上架后填写）

## 发布步骤（操作清单）

1. 在 GitHub 建一个公开仓库（名字自定；用户站用 `USERNAME.github.io`，项目站任意名）。
2. 把本站全部文件推到仓库主分支。
3. 打开仓库 Settings → Pages → Build and deployment → Source 选 "Deploy from a branch"，分支选主分支、目录选根目录（`/`）。
4. 等几分钟，打开 `https://USERNAME.github.io`（用户站）或 `https://USERNAME.github.io/仓库名/`（项目站）检查。
5. 项目站需把 `_config.yml` 里的 `baseurl` 改成 `/仓库名`；用户站留空。
6. 自定义域名（以后）：域名确定后，把 `_config.yml` 的 `url` 改成新域名；在仓库 Pages 设置里填 Custom domain；按 GitHub 提示在域名商处加 CNAME 记录；并把全站链接里的相对路径换成绝对地址（llms.txt 顶部的说明也要更新）。

## 上线前待填清单

- [x] `_config.yml`：`url`（域名）、`github_repo`（源码仓库）已填；`gumroad_url`（购买链接）待上架后填
- [ ] Gumroad 商品上架，拿到商品链接后填 `gumroad_url`
- [ ] GPU 验证后，把各工作流详情页的模型/节点/显存/成本从"待定"换成实测值，并把"ComfyUI .json 图文件待 GPU 验证"换成已验证
- [ ] 免费试用、更新政策、退款政策确认后写入定价页与 llms.txt
- [ ] 16 篇教程正文、实测对比数据、成本计算器表填写
- [ ] 目录铺开（Civitai / OpenArt 引流）时，把站链接填进各平台

## 规矩

- 不许对外宣称 ComfyUI .json 图文件已经做完、已经发布：图文件没通过 GPU 验证之前，所有工作流页都标"ComfyUI .json 图文件待 GPU 验证"；方法已定的可以写方法，不许写成图文件已有。
- 没核实的东西标"待核实"/"待定"，不编数字。
- 用户自己的内部班子是他自己的东西，绝不进站。
- 自用不卖的东西不上站、不进包，站上只写可售内容。
- 中文为主，关键处附英文。
