# reference
https://zhuanlan.zhihu.com/p/25198543
https://www.zhihu.com/question/58033789/answer/254673663
## conda in powershell
https://blog.csdn.net/qq_38163755/article/details/88144767
conda install -n root -c pscondaenvs pscondaenvs
Set-ExecutionPolicy RemoteSigned

# normal
activate // 切换到base环境

activate learn // 切换到learn环境

conda create -n learn python=3 // 创建一个名为learn的环境并指定python版本为3(的最新版本)

conda env list // 列出conda管理的所有环境

conda list // 列出当前环境的所有包

conda install requests 安装requests包

conda remove requests 卸载requets包

conda remove -n learn --all // 删除learn环境及下属所有包

conda update requests 更新requests包

conda env export > environment.yaml // 导出当前环境的包信息

conda env create -f environment.yaml // 用配置文件创建新的虚拟环境

# 创建虚拟环境
conda create -n learn python=3.8 // 创建一个名为learn的环境并指定python版本为3(的最新版本)

activate // 切换到base环境

activate learn // 切换到learn环境

# 更换清华源 装 pytorch
conda config --show

conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/pytorch/

conda config --set show_channel_urls yes

conda install pytorch torchvision cudatoolkit=10.1

# 卸载
conda install anaconda-clean

anaconda-clean --yes

uninstall.exe
