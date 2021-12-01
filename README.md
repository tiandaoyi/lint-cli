# lint-cli

使用eslint+standard+prettier+lint-staged+husky+commitlint 进行校验

注意:node版本>=12.13.0

1.eslint

        我们统一使用standard标准

配置standard规范eslint-config-standard
安装vscode插件 ESLint


2.prettier格式化代码



安装prettier
由于和eslint默认规则存在样式冲突,使用 eslint-config-prettier解决冲突
使用prettier自带规则即可
安装vscode插件 Prettier - Code formatter


3.editorconfig保持多端统一

创建.editorconfig文件
安装vscode插件 EditorConfig for VS Code


4.lint-staged对暂存区做校验



由于历史代码过多,我们使用lint-staged对添加到暂存区的文件进行校验、格式化
lint-staged要求node版本>=12.13.0
默认要求git仓库和代码文件在同一目录下
需要配合husky钩子


5.使用约定式提交Conventional Commits规范commit信息



使用commitlint校验
校验不通过,自动启动commitizen来创建交互式提交




快速生成配置文件(注: git仓库和package.json要在一个文件夹中,如果不在,在package.json目录中,使用下面命令生成后,手动修改配置文件



安装

npm install eslint-create-cli -g
eslint-create-cli init
