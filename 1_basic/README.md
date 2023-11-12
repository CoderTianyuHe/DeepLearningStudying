
# NOTE 11/11/2023 （mac）
## conda的使用

1. 创建一个虚拟环境
    conda create -n torch python=3.11
    conda activate torch
2. 明确环境有什么
    conda list // 看有哪些包
    pip install package==(version)
    conda install package==(version) 
    // 补充以及确定版本
3. 运行python文件
    python PATH // 路径

4. 注意事项：
   + 不要使用torch.py之类的名字，python会识别错误
   + 使用conda自己设定优于使用base环境

## bug avoid
遇到了模块无法识别的问题，torch下方出现波浪线
+ 解决办法：
+ 更换解释器：

    Terminal中：
    python
    import sys
    print(sys.executable)

复制路径，此时的python就是conda下的python
输入 command+shift+p 选择解释器
添加，输入路径即可
+ 此时，使用右上角的小三角运行不会报错
+ 当然，如果命令行直接python filename.py更好

## git
    //开始时复制过来
    git clone 

    // 仓库变化
    git pull https://github.com/CoderTianyuHe/DeepLearningStudying.git

    //修改完代码提交
    git remote add origin https://github.com/CoderTianyuHe/DeepLearningStudying.git
    //初始化
    git init
    git add .
    git commit -m '...'
    git push
    //git push有时需要强制执行
    git push -u origin main -f

    //查看需不需要提交
    git status



