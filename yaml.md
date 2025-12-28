基础网址: https://55220000.xyz/
语言代码: en-us
主题: hugo-theme-stack
标题: 示例站点
版权: Dryao

# 主题国际化支持
# 可用值: en,zh-cn
默认内容语言: zh-cn

# 如果 默认内容语言 在 [zh-cn ja ko] 中，则将 包含中日韩语言 设置为 true
# 这将使 .Summary 和 .WordCount 对中日韩语言正确工作
包含中日韩语言: false

语言:
    en:
        语言名称: 英语
        标题: 55220000-dryao
        权重: 1
        参数:
            侧边栏:
                副标题: 示例描述
    zh-cn:
        语言名称: 中文
        标题: 55220000-dryao
        权重: 2
        参数:
            侧边栏:
                副标题: 演示说明


服务:
    # 使用前更改为您的 Disqus 短名称
    disqus:
        短名称: "hugo-theme-stack"
    # GA 追踪 ID
    谷歌分析:
        ID:

分页:
    每页数量: 3

永久链接:
    文章: /p/:slug/
    页面: /:slug/

参数:
    主要分区:
        - post
    特色图片字段: image
    RSS完整内容: true
    网站图标: /favicon.ico
     # 例如：将网站图标放在站点文件夹的 `static/favicon.ico` 中，然后将此字段设置为 `/favicon.ico`（`/` 是必需的）

    页脚:
        起始时间: 2025-12
        自定义文本:

    日期格式:
        发布: 2006年01月02日
        最后更新: 2006年01月02日 15:04 MST

    侧边栏:
        表情符号:
        副标题: Lorem ipsum dolor sit amet, consectetur adipiscing elit.
        头像:
            启用: true
            本地: true
            源: img/avatar.png

    文章:
        数学公式: false
        目录: true
        阅读时间: true
        许可:
            启用: true
            默认: 采用 CC BY-NC-SA 4.0 许可

    评论:
        启用: true
        提供商: disqus

        disqusjs:
            短名称:
            API地址:
            API密钥:
            管理员:
            管理员标签:

        utterances:
            仓库:
            议题术语: pathname
            标签:

        beaudar:
            仓库:
            议题术语: pathname
            标签:
            主题:

        remark42:
            主机:
            站点:
            语言环境:

        vssue:
            平台:
            所有者:
            仓库:
            客户端ID:
            客户端密钥:
            自动创建议题: false

        # Waline 客户端配置参见: https://waline.js.org/en/reference/component.html
        waline:
            服务器地址:
            语言:
            页面浏览:
            表情符号:
                - https://unpkg.com/@waline/emojis@1.0.1/weibo
            必填元信息:
                - name
                - email
                - url
            语言环境:
                管理员: 管理员
                占位符:

        twikoo:
            环境ID:
            区域:
            路径:
            语言:

        # 各种选项的描述参见 https://cactus.chat/docs/reference/web-client/#configuration
        cactus:
            默认主服务器地址: "https://matrix.cactus.chat:8448"
            服务器名称: "cactus.chat"
            站点名称: "" # 您必须在此处插入一个唯一的标识符，与您注册的标识符匹配（参见 https://cactus.chat/docs/getting-started/quick-start/#register-your-site）

        giscus:
            仓库:
            仓库ID:
            分类:
            分类ID:
            映射:
            浅色主题:
            深色主题:
            反应已启用: 1
            发送元数据: 0

        gitalk:
            所有者:
            管理员:
            仓库:
            客户端ID:
            客户端密钥:
            代理:

        cusdis:
            主机:
            ID:
    小部件:
        首页:
            - 类型: 搜索
            - 类型: 归档
              参数:
                  限制: 5
            - 类型: 分类
              参数:
                  限制: 10
            - 类型: 标签云
              参数:
                  限制: 10
        页面:
            - 类型: 目录

    开放图谱:
        twitter:
            # 您的 Twitter 用户名
            站点:

            # 可用值: summary, summary_large_image
            卡片: summary_large_image

    默认图片:
        开放图谱:
            启用: false
            本地: false
            源:

    颜色方案:
        # 显示切换按钮
        切换: true

        # 可用值: auto, light, dark
        默认: auto

    图片处理:
        封面:
            启用: true
        内容:
            启用: true

### 自定义菜单
### 参见 https://stack.jimmycai.com/config/menu
### 要删除关于、归档和搜索页面菜单项，请从它们的 FrontMatter 中删除 `menu` 字段
菜单:
    主菜单: []

    社交:
        - 标识符: github
          名称: GitHub
          网址: https://github.com/CaiJimmy/hugo-theme-stack
          参数:
              图标: brand-github

        - 标识符: twitter
          名称: Twitter
          网址: https://twitter.com
          参数:
              图标: brand-twitter

相关文章:
    包含较新: true
            阈值: 60
    转小写: false
    索引:
        - 名称: 标签
          权重: 100

        - 名称: 分类
          权重: 200

标记:
    goldmark:
        扩展:
            直通:
                启用: true
                分隔符:
                    块:
                        - - \[
                          - \]
                        - - $$
                          - $$
                    行内:
                        - - \(
                          - \)
        渲染器:
            ## 如果 Markdown 中有 HTML 内容，设置为 true
            不安全: true
    目录:
        结束级别: 4
        有序: true
        开始级别: 2
    高亮:
            无类名: false
            代码围栏: true
            猜测语法: true
            行号起始: 1
            显示行号: true
            表格中显示行号: true
            制表符宽度: 4