# ybd-rn

### navigation.navigate参数

navigation.navigate('Home', {
  screen: 'Feed',
  params: { 
    sort: 'latest'
     },
});

项目运行:
  yarn
  cd ios && pod install


M1芯片
如果pod install 报错 运行
#### cd ios && arch -x86_64 pod install


android启动项目

在ybd-rn/node_modules/react-native-picker/android/build.gradle中，
### 把底部两个 compile 改为 implementation

ybd-rn/android/settings.gradle中添加：
include ':react-native-picker'
project(':react-native-picker').projectDir = new File(rootProject.projectDir, '../node_modules/react-native-picker/android')