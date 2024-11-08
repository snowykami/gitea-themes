# 自制的Gitea主题集合

## 安装

1. 二进制部署的将`custom`目录放到`/var/lib/gitea`，此后看起来应该是`/var/lib/gitea/custom/**`
2. docker或docker compose部署的请放到`/var/lib/gitea`挂载的目标目录下

## 使用
1. 二进制部署请编辑`/etc/gitea/app.ini`，docker部署的请编辑对应挂载目录下的`app.ini`
添加如下两个新主题，一个蓝色系，一个粉色系

```ini
[ui]
THEMES = ...,snowykami,liteyuki-magipoke
DEFAULT_THEME = liteyuki-magipoke  # 可选
```
2. 重启gitea
3. 进入个人设置>外观>主题，下拉即可看到新主题，选择应用后即可生效

## 展示
实例: [git.liteyuki.icu](https://git.liteyuki.icu)
![image](https://github.com/user-attachments/assets/7c33d333-d6be-498b-8492-888b560a8d97)
