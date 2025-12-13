# auto-login-clawcloud
每15天自动登录爪云保活，需要关闭passkey和开启2FA
进入您的 GitHub 仓库 -> Settings -> Secrets and variables -> Actions -> New repository secret。

开启 GitHub 2FA 并获取密钥：

去 GitHub 设置 -> Password and authentication -> Enable 2FA。

关键： 点击复制二维码下方，Setup Key蓝色字体获取那串字符密钥，通常是 16 位的字母数字组合。

配置 GitHub Secrets： 在您的仓库 -> Settings -> Secrets and variables -> Actions 中添加以下 3 个 Secret：

GH_USERNAME: 你的 GitHub 账号（邮箱）。

GH_PASSWORD: 你的 GitHub 密码。

GH_2FA_SECRET: 刚才复制的那串 2FA 密钥 (去掉空格)。
