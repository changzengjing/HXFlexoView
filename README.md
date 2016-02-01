# HXFlexoView
一个非常牛B的View!
大家经常做项目,应该会遇到一个界面的一行有多个UILaebl 多个UIImageView混的情况,尤其是UILaebl的文字长度是动态的情况,这时候就需要计算各种长度位置,比较麻烦,关键是,这种情况非常常见,所以我就想出来写这么一个多功能View,它基本上满足你日常大部分需求,不管是一行一个UILabel还是2个UILabel,或者是一个UIImageView或者2个,或者UILabel与UIImageView组合,只要你想的到的,HXFlexoView都可以满足你.如果你觉得对你有用,记得给点个赞哦,谢谢!您的支持,是我最大的动力.欢迎关注本人博客: http://blog.libuqing.com/

# 效果图
![image](https://github.com/huangxuan518/HXFlexoView/blob/master/HXFlexoView/xiaoguo.gif)

# 参数说明图
![image](https://github.com/huangxuan518/HXFlexoView/blob/master/HXFlexoView/tushi.png)

# 用法示例
    HXFlexoView *flexoView = [[HXFlexoView alloc] initWithFrame:CGRectMake(_icoImageView.frame.origin.x + _icoImageView.frame.size.width + 10, _icoImageView.frame.origin.y, self.view.frame.size.width-20 - _icoImageView.frame.size.width - 10, 17)];
    flexoView.alignment = 2;//对齐方式 默认左对齐,可不设置
    flexoView.leftLabel.text = @"黄轩";//设置则显示,不设置则不显示
    flexoView.leftImageView = [[UIImageView alloc] initWithImage:[UIImage imageNamed:@"qq_xunzhang"]];//设置则显示,不设置则不显示
    flexoView.rightImageView = [[UIImageView alloc] initWithImage:[UIImage imageNamed:@"qq_wifi"]];//设置则显示,不设置则不显示
    flexoView.rightLabel.text = @"冬季到台北来看雨";//设置则显示,不设置则不显示
    [self.view addSubview:flexoView];
