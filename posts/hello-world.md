# Hello World

这是我的第一篇博客文章。

## 关于这个博客

这个博客基于 Markdown 构建，支持以下特性：

- **代码高亮** — 支持多种编程语言
- **数学公式** — 可扩展 KaTeX 支持
- **GFM 语法** — 表格、任务列表等
- **响应式设计** — 适配各种屏幕

## 代码示例

```python
import torch
import torch.nn as nn

class SimpleTransformer(nn.Module):
    def __init__(self, d_model=512, nhead=8):
        super().__init__()
        self.attention = nn.MultiheadAttention(d_model, nhead)
        self.norm = nn.LayerNorm(d_model)

    def forward(self, x):
        attn_out, _ = self.attention(x, x, x)
        return self.norm(x + attn_out)
```

## 如何发布新文章

1. 在 `posts/` 目录下创建 `.md` 文件
2. 在 `posts/posts.json` 中添加文章元信息
3. 推送到 GitHub，完成发布

> 写作是思考的最佳方式。

---

欢迎来到我的博客，未来会在这里分享机器学习笔记、项目心得和技术思考。
