# unfo-term
```
https://vivaldi.club 论坛终端浏览器
用于在非桌面环境里访问vivaldi论坛
全部为bash脚本，不需要任何json解释器
如果安装了fbterm则可以在tty中使用
支持登陆/浏览/发帖/回帖
2017-02-11 15:00

usage:
b.unfo # 打开首页帖子列表
op=N  b.unfo # 打开帖子列表第N个分页
b.unfo  [discussionId]  [page] # 打开指定帖子的指定页码
i.unfo  [user]  [pw] # 以用户名user和密码pw登陆并将得到的token记录到文件以备使用
r.unfo  [discussionId]  [text] # 以默认用户名回帖
ouser=xyz  r.unfo  [discussionId]  [text] # 以用户名xyz(限事先以unfo.i成功登陆过的id)回帖
iscode=1   r.unfo  [discussionId]  [text] # 自动为回帖内容添加ubb[code]标记
p.unfo  [tagId]  [title]  [text] # 在指定tagId下发布新话题
ivid='00,000'  p.unfo  [tagId]  [title]  [text] # 在指定tagId下发布只有userId为00和000的用户可见的新话题
ivuer='u1,u2'  p.unfo  [tagId]  [title]  [text] # 在指定tagId下发布只有userName为u1和u2的用户可见的新话题
xyz [--help|-h|--tags|-t] # 通用文件,显示帮助或tag列表
```
# 首次使用前请修改 xyz 文件或在当前shell中 export ouser=xxx 来指定默认用户名以提高效率

