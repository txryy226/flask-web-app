# flask-web-app

通过 GitHub Actions 实现 Flask Web 项目的自动化构建、测试与部署，最终将项目自动部署至头歌（Educoder）服务器。

## 项目结构

```
flask-web-app/
├── src/
│   ├── app.py          # Flask 核心应用代码
│   └── __init__.py     # 空文件
├── tests/
│   └── test_app.py     # 测试用例
├── .github/
│   └── workflows/
│       └── cicd.yml    # GitHub Actions 工作流配置
├── requirements.txt    # 项目依赖清单
└── README.md
```

## 流程

推送代码到 `main` 分支 → GitHub Actions 自动跑测试 → 通过 SSH 部署到头歌服务器 → 重启 Flask 服务。
