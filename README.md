## 概念

> The Conventional Commits specification is a lightweight convention on top of commit messages. It provides an easy set of rules for creating an explicit commit history; which makes it easier to write automated tools on top of.
>
> 约定式提交规范（Conventional Commits specification）是针对提交信息（commit message）的轻量化解决方案。该方案提供了一组简明规定，目的使提交过程中的历史信息清晰、有条理，编写基于该归规定的自动化工具更加轻松。
>
> ——[Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)

## 工具

通过以下工具实现 [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)

-   自动生成提交信息

    -   [commitizen](https://github.com/commitizen/cz-cli)：自动生成提交信息，需要配置模板
    -   [cz-conventional-changelog](https://github.com/commitizen/cz-conventional-changelog)：提交模板（adapter）

-   检测提交信息是否符合规范
    -   [husky](https://github.com/typicode/husky#readme)：提供 git 钩子函数，用于在成功提交信息前调用 commitlint
    -   [commitlint](https://github.com/conventional-changelog/commitlint#readme)：检测是否符合规范，需要配置模板
    -   [commitlint/config-conventional](https://github.com/conventional-changelog/commitlint/tree/master/%40commitlint/config-conventional#type-enum)：检测模板

## 流程

1. git pull
2. git add .
3. npm run commit

## 参考

-   [如何配置 Git Commit Message - 知乎](https://zhuanlan.zhihu.com/p/69635847)
-   [ConversationLearner-UI/package.json at master · microsoft/ConversationLearner-UI](https://github.com/microsoft/ConversationLearner-UI/blob/master/package.json)
