# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'Jirachi' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for Jirachi

  pod 'DoraemonKit/WithLogger', '1.1.3', :configurations => ['Debug']
  
  # Pods for React Native
  pod 'React', :path => './Jirachi-RN/node_modules/react-native', :subspecs => [
  'Core',
  'CxxBridge', # 如果RN版本 >= 0.47则加入此行
  'DevSupport', # 如果RN版本 >= 0.43，则需要加入此行才能开启开发者菜单
  'RCTText',
  'RCTNetwork',
  'RCTWebSocket', # 调试功能需要此模块
  'RCTAnimation', # FlatList和原生动画功能需要此模块
  # 在这里继续添加你所需要的其他RN模块
  ]
  # 如果你的RN版本 >= 0.42.0，则加入下面这行
  pod "yoga", :path => "./Jirachi-RN/node_modules/react-native/ReactCommon/yoga"
  # 如果RN版本 >= 0.45则加入下面三个第三方编译依赖
  pod 'DoubleConversion', :podspec => './Jirachi-RN/node_modules/react-native/third-party-podspecs/DoubleConversion.podspec'
  pod 'glog', :podspec => './Jirachi-RN/node_modules/react-native/third-party-podspecs/glog.podspec'
  pod 'Folly', :podspec => './Jirachi-RN/node_modules/react-native/third-party-podspecs/Folly.podspec'

  target 'JirachiTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'JirachiUITests' do
    inherit! :search_paths
    # Pods for testing
  end

end
