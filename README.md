<h1 align="center">🌟天眼查脚本</h1>


## 使用指南：
需要网页登录天眼查后，替换脚本中的三个cookie。如果账号是淘宝临时的，当你在使用时别人登陆了，那么cookie会立马失效。执行完tyc_structure.py 和 tyc_group.py 对应域名和邮件拿出来去重即可食用。


tyc_structure.py
主要就是这个脚本，在脚本中设置下级公司占股比例，一般50即可。在使用过程中，大概率会触发二次校验，可根据脚本给的提示进行操作。
主要生成3个文件：
structure_assets.csv    占股比例逻辑表 及 对应公司相关域名、相关注册邮箱
structure_CompaniesList.csv  所有公司名
structure_urls.csv   对应公司域名
structure_emails.csv   对应公司邮箱

tyc_group.py
此脚本爬取目标公司对应的集团子公司，主要应对一种情况：A公司有10家集团公司共同控股，但是控股比例低，因此tyc_structure.py 收录不到。
主要生成3个文件：
group_CompaniesList.csv    集团公司域名及注册邮箱
group_urls.csv  集团公司域名
group_emails.csv   集团公司邮箱


tyc_dremove.py
此脚本主要负责筛选 tyc_group.py 脚本对应的公司，此类公司可以额外关注，如有需求可以使用tyc_structure.py 进行股权爬取。

BY:CT

/result

![image](https://user-images.githubusercontent.com/48993128/171550824-bbe46156-2cbc-4fbd-b550-2febffe0a394.png)

+ structure_assets.csv    占股比例逻辑表 及 对应公司相关域名、相关注册邮箱

![image](https://user-images.githubusercontent.com/48993128/171551179-b0d6317b-c89e-4675-84fe-593e6d9ea57b.png)

