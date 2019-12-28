# PBAC-power RBAC权限后台角色与权限设计
## 随着业务与用户量起来后。都会考虑系统的角色与权限设计。借此经典的角色与权限设计：RBAC，基于角色的权限访问控制。
### 项目的内容是搭建后台对前台用户及用户角色授权以及菜单对功能模块的分类的管理。其实核心就是将账号、角色权限、菜单链接起来的设计方式；
### 功能设计：
#### 1）用户通过B/S结构的后台系统通过不同的账号判断出背后的角色，到底这个角色包含那些权限去访问模块1、	资源2、菜单3等。（我将用2个不同的用户演示）
#### 2）在该账户所在的角色下，如果没有该模块的权限，用户将无法使用。相反，即可使用。上诉的流程就保证了用户操作权限。
#### 3）后台超级管理员可以可以创建各种角色，每种角色也都可以授权各种权限菜单等。
#### 4）除了系统开发者外，没有人能创建超级管理员。这是为了系统的安全性设想的。以及用户访问只能从登陆

### 界面展示：

##### 后台管理员登录界面（这次用超级管理员账号登录）
![后台管理员登录界面](https://github.com/qiang5201/PBAC-power/blob/master/img/%E7%AE%A1%E7%90%86%E5%91%98%E7%99%BB%E5%BD%95.png)

##### 超级管理员界面
![超级管理员界面](https://github.com/qiang5201/PBAC-power/blob/master/img/%E8%B6%85%E7%BA%A7%E7%AE%A1%E7%90%86%E5%91%98%E7%95%8C%E9%9D%A2.png)

##### 收搜功能
![收搜功能](https://github.com/qiang5201/PBAC-power/blob/master/img/%E6%94%B6%E6%90%9C%E5%8A%9F%E8%83%BD.png)

##### 用户角色授权功能
![用户授权功能](https://github.com/qiang5201/PBAC-power/blob/master/img/%E7%94%A8%E6%88%B7%E8%A7%92%E8%89%B2%E6%8E%88%E6%9D%83.png)

##### 角色管理功能
![角色管理功能](https://github.com/qiang5201/PBAC-power/blob/master/img/%E8%A7%92%E8%89%B2%E7%AE%A1%E7%90%86%E7%95%8C%E9%9D%A2.png)

##### 超级管理员角色（拥有全部菜单权限）
![超级管理员角色](https://github.com/qiang5201/PBAC-power/blob/master/img/%E8%B6%85%E7%BA%A7%E7%AE%A1%E7%90%86%E5%91%98%E8%A7%92%E8%89%B2.png)

##### 一般管理员角色（拥有部分菜单权限）
![一般管理员角色](https://github.com/qiang5201/PBAC-power/blob/master/img/%E4%B8%80%E8%88%AC%E7%AE%A1%E7%90%86%E5%91%98%E8%A7%92%E8%89%B2.png)

##### 菜鸟角色管理员（拥有部分菜单权限）
![菜鸟角色管理员](https://github.com/qiang5201/PBAC-power/blob/master/img/%E8%8F%9C%E9%B8%9F%E8%A7%92%E8%89%B2%E7%AE%A1%E7%90%86%E5%91%98.png)

##### 系统菜单管理（可以自己添加菜单，需要选择左边的目录，或者选中顶级目录）
![系统菜单管理](https://github.com/qiang5201/PBAC-power/blob/master/img/%E7%B3%BB%E7%BB%9F%E8%8F%9C%E5%8D%95%E7%AE%A1%E7%90%86.png)

##### 后台管理员登录界面（这次用菜鸟管理员账号登录）
##### 我们看到这次只显示人员管理菜单，那是因为这个用户只有菜鸟管理员角色，而这个角色只能看到权限管理下的人员管理，如果想获得更多菜单，那就要授权了！
![菜鸟管理员登录](https://github.com/qiang5201/PBAC-power/blob/master/img/%E8%8F%9C%E9%B8%9F%E7%AE%A1%E7%90%86%E5%91%98%E7%99%BB%E5%BD%95.png)

## End~
