# StretchHeader
this is a stretchable view in tableviewHeader,enlarge the view 

这是一个可拉伸的view，主要放在UITableView的header处。
该功能是基于HFStretchableTableHeaderView作修改的，使得放在头部的view可以向下和向左右拉伸。
用于：
    一些使用tableview的“个人界面”；
    需要拉伸图片功能的tableview的头部；
使用：
- (void)stretchHeaderForTableView:(UITableView*)tableView
                         withView:(UIView*)view
                         subViews:(UIView*)subview;

实现该方法－－view：是放拉伸的背景图片，也可以自定义一个UIView。subview：放在view之上的，可自定义subView，也可直接实例一个透明的subview。

*记得实现以下两个代理方法
- (void)scrollViewDidScroll:(UIScrollView *)scrollView
- (void)viewDidLayoutSubviews

如果你觉得有更好的，可以试着再改一下哦～