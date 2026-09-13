# 博客

个人博客站点，Next.js + Tailwind CSS 构建的毛玻璃（Glassmorphism）风格前端。

- 线上地址：<https://513613.qzz.io>
- 站点内容：文章 / 杂谈 / 说说 / 归档 / 照片墙 / 音乐 / 友链 / 关于
- 内容以 Markdown 存放在仓库内的 `posts/`、`chatters/`、`moments/` 目录，站点配置集中在 `siteConfig.ts`

## 技术栈

- **框架**：Next.js 16（App Router）
- **样式**：Tailwind CSS 4
- **内容解析**：gray-matter + remark/rehype（支持 Markdown 与 KaTeX 公式）
- **动效**：framer-motion、three.js（@react-three/fiber）
- **部署**：Vercel，域名经 Cloudflare 代理

## 本地开发

```bash
npm install
npm run dev      # 开发模式，默认 http://localhost:3000
npm run build    # 生产构建
npm start        # 运行生产构建
```

## 内容与配置

| 路径 | 说明 |
| --- | --- |
| `posts/*.md` | 文章，frontmatter 支持 `title` / `date` / `description` / `cover` / `tags` |
| `chatters/*.md` | 杂谈 |
| `moments/*.md` | 说说（含 `images` 数组） |
| `data/albums.ts` | 相册数据 |
| `data/friends.ts` | 友链数据 |
| `data/projects.ts` | 项目数据 |
| `app/about/about.md` | 关于我 |
| `siteConfig.ts` | 全站配置：站名、头像、背景、社交入口、弹幕、音乐等 |
| `public/` | 静态资源（头像、背景图、封面等） |

## 部署

推送到 `main` 分支后，Vercel 会自动构建并发布到生产环境，无需手动操作。

## 许可证

本项目基于 [XinghuisamaBlogs](https://github.com/heiehiehi/XinghuisamaBlogs)（CC BY-NC 4.0）二次修改使用，仅供个人非商业用途。
