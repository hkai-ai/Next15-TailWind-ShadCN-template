该仓库为元狲科技的前端工程创建模板。仅供参考使用。

## 1.0 特性

具有的特性：

| Feature      | 描述                                                                                        |
| ------------ | ------------------------------------------------------------------------------------------- |
| Next.js      | Version 14.2.3                                                                                  |
| TailwindCSS  |                                                                                             |
| ShadCN-UI    | 之后直接运行组件安装的 npx CI 即可安装相应组件                                              |
| Merge-bot    | 自带Merge-bot，如果不想要，删除 .github 文件夹即可。如果使用，需要在 issue 里添加相关标签。 |
| VSCode Debug | 可通过 VSCode 进行全栈 debug                                                                |

### 1.1 Next.js 特性

- App Router，该模板启用的是 App Router。不建议使用 Pages Router。

## 2.0 更新日志

### v0.2.0 - Next.js 15 升级 (2026-03-16)

将模板从 Next.js 14 升级至 Next.js 15，同步升级 React 至 v19。

#### 依赖变更

| 依赖               | 旧版本   | 新版本   |
| ------------------ | -------- | -------- |
| next               | 14.2.35  | 15.5.12    |
| react              | ^18      | ^19      |
| react-dom          | ^18      | ^19      |
| @types/react       | ^18      | ^19      |
| @types/react-dom   | ^18      | ^19      |
| @types/node        | ^20      | ^22      |
| eslint-config-next | 14.2.3   | ^15.2    |
| lucide-react       | ^0.378.0 | ^0.475.0 |

#### 升级说明

- **React 19**：Next.js 15 要求 React 19，带来了新的编译器优化和改进的 Server Components 支持。
- **lucide-react**：旧版本不兼容 React 19，已升级至支持 React 19 的版本。
- **ESLint**：保持 ESLint 8，未迁移至 ESLint 9 flat config 格式。`eslint-config-next` 已同步升级至 v15。
- **无破坏性变更**：本模板未使用 Next.js 15 中有 breaking changes 的 API（如 async `cookies()`、`headers()`、`params`、`searchParams`），因此无需修改业务代码。
