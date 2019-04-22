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

• employee_citizenship: 员工国籍

## 思路整理：
1. 对数据进行探索性分析，观察数据完整性和特征。
2. 对缺失值进行填充处理，新增一列特征‘annual—wage’，作为目标变量计算雇员的年薪。
3. 删除‘annual—wage’中的异常值，对其进行对数变换。
4. 对原数据集中的类型特征做one－hot处理，并求出每一类别下的平均年薪，用以输入预测模型。
5. 分别用线性回归和随机树模型对数据集进行拟合，评估模型效果。

## 模型效果
1. 线性回归模型：

  MAE: 11897.598067391895
  MSE: 1840392219.8896956
  RMSE: 42899.792772106666

2. 随机森林模型：

  MAE: 7233.704545409459
  MSE: 216472254.0654224
  RMSE: 14712.99609411429
