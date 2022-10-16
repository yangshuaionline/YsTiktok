#[GitHub地址](https://github.com/yangshuaionline/YsTiktok)
#目录：
1. ####[项目结构](#list1)
2. ####[模块说明](#list2)
3. ####[近期安排](#list3)

##<a id="list1">1. 项目结构</a>：
+ [app](#app)：聚合模块
    - [module_main](#module_main)：main业务功能模块
    - [功能模块2](#test2)：具体业务功能模块块
        * [base](#base)：聚合组件
            + [library_constant](#library_constant)：提供模块之间交互变量
            + [library_video](#library_video)：视频播放模块，对外暴露使用接口


##<a id="list2">2. 模块说明</a>：

+ ###<a id="app">app</a>：
  >1. 程序入口
  >2. 合并所有功能模块
  >3. gradle内部使用implementation
+ ###<a id="module_main">module_main</a>：
  >1. 封装主页模块
  >2. 使用Arouter跳转其他页面
  >3. gradle内部使用api
  >4. 使用的时候注意在[library_constant](#library_constant)对应文件夹下定义接口
+ ###<a id="test2">功能模块2</a>：
  >1. 封装功能模
  >2. gradle内部使用api
  >3. 使用的时候注意在[library_constant](#library_constant)对应文件夹下定义接口
+ ###<a id="base">base</a>：
  >1. 集成组件
  >2. 封装公有功能
  >3. 存放公共资源
  >4. gradle内部使用api 
+ ###<a id="library_constant">library_constant</a>：
  >1. 负责提供跨模块公共常量的维护
  >2. 负责各模块Arouter路由的暴露
  >3. 使用的时候注意每个模块在单独的一个文件夹下
+ ###<a id="library_video">library_video</a>：
  >1. 负责处理视频播放相关功能
  >2. 内部功能闭环，对外提供使用接口
  >3. gradle内部使用apiimplementation

##<a id="list3">3. 近期任务安排</a>：
- [x] 框架结构安排
- [ ] 框架引入Databinding
- [ ] 框架引入Arouter
- [ ] 编写base层
    - [ ] 编写main层
    - [ ] 编写video层
    
        
            
                


