# 选择题9
## 假设京东物流所有的运单信息都存储在一张名为waybill_info的运单表中，请找出配送站点（site_name）名称为京东总部4号楼，并且运单状态（waybill_state）超过3次为妥投异常的所有运单号（waybill_code）


</br>


### **A** select waybill_code,count(*) from waybill_info where site_name="京东总部4号楼" and waybill_state='妥投异常' and count(waybill_code)>3;<br>
### **B** select waybill_code from waybill_info where site_name="京东总部4号楼" and waybill_state='妥投异常' group by waybill_code having count(*)>3;<br>
### **C** select waybill_code from waybill_info where site_name="京东总部4号楼" and waybill_state='妥投异常' and having count(*)>3;<br>
### **D** select waybill_code,count(*) from waybill_info where site_name="京东总部4号楼" and waybill_state='妥投异常'  order by waybill_code having count(*) >3