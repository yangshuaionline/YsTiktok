- [GitHub](https://github.com/yangshuaionline/YsTiktok)






#项目结构：
+ `==gradle内部使用implementation==`
+ app：
    >1. 程序入口
    >2. 合并所有功能模块
    - `==gradle内部使用api==`
    - module_main：
      >1. 封装主页模块
      >2. 使用Arouter跳转其他页面
      >3. 使用的时候注意在[library_constant](#library_constant)对应文件夹下定义接口
    - `==gradle内部使用api==`
    - 功能模块2：
      >1. 封装功能模
      >2. 使用的时候注意在[library_constant](#library_constant)对应文件夹下定义接口
      * `==gradle内部使用api==`
      * module_base：
        >1. 集成组件
        >2. 封装公有功能
        >3. 存放公共资源
        + `==gradle内部使用implementation==`
        + <a id="library_constant">library_constant</a>：
          >1. 负责提供跨模块公共常量的维护
          >2. 负责各模块Arouter接口的暴露
          >3. 使用的时候注意每个模块在单独的一个文件夹下
        + `==gradle内部使用implementation==` 
        + library_video：
          >1. 负责处理视频播放相关功能
          >2. 内部功能闭环，对外提供使用接口

        
            
                


