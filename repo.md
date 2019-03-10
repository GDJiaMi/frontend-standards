# 版本库规范

> TODO: 文档待完善

## 命名

- 基础库
  - @gdjiami/{NAME}
- 业务项目
  - gzb-{NAME}

## 文件结构

- README.md: 项目说明
- CHANGELOG.md
  - 放置每个版本的变动内容
    - 包含内容
      - 新增的功能
        - break change需要特别说明
      - bug修复
    - 生成器
      - conventional-changelog
    - 规范
      - KeepAChangelog
- package.json: 保持version字段和当前版本同步.
- .gitignore
- docs/: 细化文档
- dist/: 项目构建结果输出目录
- src/: 源代码目录
- \_\_tests\_\_/: 单元测试目录. 和被测试的模块在同一个父目录下
- .env*
  - 项目构建/开发配置文件. 不要变动’非.local文件’, 避免影响其他开发者, 如果需要变动, 应该建立自己的.local文件. 例如.env.development.local
- [其他细节](https://carney520.github.io/jm-cli/docs/folder-structure)