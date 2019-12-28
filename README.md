# PBAC-power RBAC权限后台角色与权限设计
## 随着业务与用户量起来后。都会考虑系统的角色与权限设计。借此经典的角色与权限设计：RBAC，基于角色的权限访问控制。
### 项目的内容是搭建后台对前台用户及用户角色授权以及菜单对功能模块的分类的管理。其实核心就是将账号、角色权限、菜单链接起来的设计方式；
### 功能设计：
#### 1）用户通过B/S结构的后台系统通过不同的账号判断出背后的角色，到底这个角色包含那些权限去访问模块1、	资源2、菜单3等。（我将用2个不同的用户演示）
#### 2）在该账户所在的角色下，如果没有该模块的权限，用户将无法使用。相反，即可使用。上诉的流程就保证了用户操作权限。
#### 3）后台超级管理员可以可以创建各种角色，每种角色也都可以授权各种权限菜单等。
#### 4）除了系统开发者外，没有人能创建超级管理员。这是为了系统的安全性设想的。以及用户访问只能从登陆

### 界面展示：
##### 后台管理员登录界面（这次用超级管理员）
![后台管理员登录界面]
