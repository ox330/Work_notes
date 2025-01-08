### 1/16
    直接供应商1600个，间接供应商15000个（物流，保洁）
    管理直接物料供应商
    已有平台SAQ,完整社会审核
    要求部分供应商进行审核，去年完成几十家 
    完成问卷需要付费

    在线SAQ问卷，基于商业，安全生产、环境保护、反腐败、劳工、劳动保护、冲突制裁
    评一个等级，反馈整改
    供应商自我评估得出等级

    不同的品牌不同的供应商，管理劳工风险，让供应商自己承担费用，

    做基础，针对不同的条款发展不同的问卷，在发达国家

    供应商直接找新亚做问卷，新亚检测一些时间，给客户一些时间核实

    想要审核供应商，让供应商进行自评，供应商分为直接或间接两类，类别不同问卷项不同

    两类
    王总提供需求和检查项，主要分为直接供应商和间接供应商问卷两类




### 1/17
todo
* 自己开通微软的Azure的GPT-4服务
* 完成24年会总结
* 升级VScode
* 翻译CDB文档
  
#### 
![]()，符号都是英文格式，其中[]中写插入的图片名称，当然也可以不写，()中填图片地址，可以是网址，也可以是本地文件的绝对路径，博文中是放在本md文件相同文件夹下，所以前面是./

安装了MPE的小伙伴参考一下这个@import <文件名>

@import<>

docker cp /home/ESG/new_asia/dispose/mysql/my.cnf bc:/etc/mysql/my.cnf

### 1/8

#### ESG部署
所有容器都正常启动以后
/home/new_asia/ pip install sqlalchemy[asyncio]
 while read requirement: ;do pip install $requirement:done < requirements.txt   (在dockefile中配置镜像源使安装更快)

 最后一步：初始数据，执行系统初始化脚本，把图表，item等刷新进去：python ./scripts/system_initialize.py

访问网站查看数据是否刷进去
最后使用nohup在后台启动程序，进程数为4
nohup gunicorn main:app --workers 4 --worker-class uvicorn.workers.UvicornWorker --bind 0.0.0.0:8000