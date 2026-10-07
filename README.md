# 分镜大师 · 技能与创作知识库

在线打开：**https://guantou33.github.io/fenjing-dashi/**

一个单文件网页知识库，红白配色，白底为主、红色点缀。电脑手机都能开，长期有效，随更新自动同步。

## 里面有什么

- 目录：17 组、137 篇，一眼看全，点标题直接进正文，鼠标移上去右边出现「⇩」可以只下这一篇
- 作品表 · 图库：首页轮播，可切网格，点开看大图/播放；每件都能单独下载原件
- 细分分类浏览：去 AI 味 / 人物三视图 / 分镜 / 运镜 / 灯光 / 表演 / 审片 / 连续性 / 剧本写作 / 提示词 / 出图出片工具链 …
- 全文搜索，点开任意一篇看正文
- 每个分类一键打包成 zip 下载，另有「全部下载」整包；每篇也能单独下载（单文件 .md，多文件 .zip）
- 分镜大师包 = 分镜师 3.0 + H3 官方提示词 + 分镜全套技能，下完直接丢进别的 agent 的 skills 目录即可用
- 剧本与创作内容（大纲、brief、视觉风格、决策记录）在里面；相关的成片视频/照片体积太大不放进网页，需要时向作者索取
- 作品表可以自己在网页上传：打开 `upload.html`，填一次 GitHub token（只存在自己浏览器里），之后拖文件就能传

## 目录

    index.html           知识库网页本体（单文件，离线也能开）
    upload.html          自助上传页（把作品直接传进这个仓库）
    media/index.json     作品表示例数据
    media/works.json     你从网页上传的作品清单（网页自动维护）
    media/t/  media/f/   缩略图 / 网页用大图
    downloads/           各分类与全量的 zip 包（永久直链）
    pack-fenjing-dashi.zip      分镜大师
    pack-quaiwei.zip            去AI味 · 真人感
    pack-renwu-sanshitu.zip     人物三视图 · 角色设定
    pack-juben.zip              剧本写作全流程
    pack-wode-chuangzuo.zip     我的创作 · 青苹果与红苹果
    pack-gongjulian.zip         出图出片工具链
    all-full.zip                全部内容

## 怎么用

1. 直接打开网页浏览、搜索、下载。
2. 要装进别的 agent：下载对应 zip，解压后把里面的 skill 文件夹放进该 agent 的 `skills/` 目录。
3. 想离线带着走：把 `index.html` 存下来即可，单文件自带全部内容。
4. 想自己传作品：打开 `upload.html` → 填仓库名和 token → 拖文件 → 等 1 分钟 Pages 重建。

## 说明

- 内容来自本机技能库与创作目录，自动同步：本机每 6 小时检查一次，有变化才重新上传，链接永久不变。
- 手动同步：在本机跑 `python deploy_fast.py`（在 `C:\Users\111\Desktop\AI\知识库` 下，只传变化的文件，秒级完成）。
- 网页里的「打包下载」按钮在本地离线打开时也能用（浏览器内即时打包）。
- token 只保存在你浏览器的 localStorage 里，用来调 GitHub 接口写这个仓库；建议用只勾选本仓库、只给 Contents 读写权限的 fine-grained token。
