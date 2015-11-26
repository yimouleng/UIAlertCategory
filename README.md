# UIAlertCategory

简单的 UIAlert 封装	如果 (iOS <= 7)使用 UIAlertView 如果 (iOS >= 8) UIAlertViewController.



## 安装

导入 `UIAlertCategory.m` 和 `UIAlertCategory.h` 并加入头文件
## 使用方法和示例
```

 UIAlertCategory * a = [[UIAlertCategory alloc] initWithTitle:@"警告" WithMessage:@"你有条警告"];
 
 [a addButton:ALERT_BUTTON_OK WithTitle:@"好的" WithAction:^(void *action) {
        NSLog(@"你点击了 index 为 0 的  好的");
 }];
 [a addButton:ALERT_BUTTON_CANCEL WithTitle:@"取消" WithAction:^(void *action) {
        NSLog(@"你点击了 index 为 1 的  取消");
 }];
 [a show];
 
 
   PS： OK 和 OTHER 目前是一样的
 
有三种 Button:
- `ALERT_BUTTON_CANCEL` alert
- `ALERT_BUTTON_OK`
- `ALERT_BUTTON_OTHER`
 
可自行添加其他Button

```