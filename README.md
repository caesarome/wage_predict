# wage_predict

## 项目背景介绍：

美国雇主可以为自己外籍员工向美国劳工部申请工作许可。雇主提交的申请中需要包含员工的个人信息和工作信息。在本项目中需要对数据进行清洗和缺失值处理，进而建模预测申请通过的员工年薪是多少。这里选用的是现行回归和随机数模型。随机数模型的效果更好。

数据字典如下:

• case_number: 雇主提交的申请的ID

• case_received_date: 申请提交的时间

• decision_date: 申请结果公布时间

• case_status: 申请结果

• employer_name: 雇主名称

• employer_num_employees: 公司的雇员数目

• employer_yr_established: 公司成立的年份

• job_education: 员工受教育程度

• job_experience_num_month: 工作要求的工作年限（按月计算）

• job_state: 工作所在地

• job_foreign_lang_req: 职位是否需要外语

• job_level: 职称

• employee_citizenship: 雇主国籍

• wage_offer: 薪水（数值）

• wage_unit: 薪水的计算单位
