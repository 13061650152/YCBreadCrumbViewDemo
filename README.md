# YCBreadCrumbView

这是一个简单实用的面包屑控件
===
USAGE
----
* set up
```
    NSArray *array = @[@"这是第一级", @"这是第二级", @"这是第三级", @"这是第四级这是第四级", @"这是第五级"];
    
    YCBreadCrumbView *breadView = [[YCBreadCrumbView alloc]initWithFrame:CGRectMake(30, 200, 300, 40)];
    breadView.backgroundColor = [UIColor grayColor];
    breadView.delegate = self;
    [self.view addSubview:breadView];
    
    [breadView setItems:array];
```
* delegate
```
- (void)breadCrumbView:(YCBreadCrumbView *)view didTapItemAtIndex:(NSInteger)index{
    NSLog(@"%ld", (long)index);
}
```
ScreenShot
---
![bbb](https://github.com/13061650152/YCBreadCrumbView/blob/master/IMG_0892.PNG "aaa")
