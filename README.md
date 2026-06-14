# ZJU OC 生存指北

手册链接：https://zjuocer.github.io/zjuoc-livingmanual/ 

本组织目前只有一个仓库。如果你有仓库想放在这个组织下，请联系组织维护者。

## 手册希望包含的内容

本手册目前着重于**舟山校区生活**方面的内容。后续希望扩展至**海洋学院独有的课程**、**海洋学院必修的外学院专业课**、**毕业去向**等内容。

本手册目前暂不收录**通识课**等内容。

## 如何参与编写

### 方法一：投稿至校内论坛 / 仓库维护者

可以在校内论坛的“海洋学院”版面发帖，注明投稿至海洋学院生存指南。也可以直接联系仓库维护者。

### 方法二：自行编写

1. 在电脑上安装 Git 和 Python （其中 Python 建议使用版本管理工具，比如 uv）。
2. 先将本仓库 `Fork` 到你的账户下，之后 `clone` 到本地。
3. 根据对应的版本管理工具安装 Zensical，可参见 [Zensical 官网](https://zensical.org/docs/get-started/)。

    pip：
    ```shell
    python -m venv .venv  
    .venv\Scripts\activate
    pip install zensical
    ```

    uv:
    ```shell
    uv init
    uv add --dev zensical
    uv run zensical
    ```

4. 输入
    ```shell
    zensical serve
    ```

    或者

    ```shell
    uv run zensical serve
    ```

    等到出现提示 `Serving ... on http://localhost:8000` 时，即可在对应的网址打开本地预览。

5. 在你想完善的文章中直接修改，保存后浏览器中将会实时更新。

6. 编辑完成后，执行

    ```shell
    git add .
    git commit -m "一句话描述本此次改动的内容"
    git push
    ```

7. 之后，在 Github 上创建 Pull Request，维护者会审查此次提交，并最终决定是否合并至主线。
