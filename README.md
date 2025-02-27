
# Run
```
bench start
```
# browse url 
```
http://erp.localhost:8000/app/

or  

http://masum.localhost:8000/app/

```

user: Administrator
password: testpass1234

bench new-site masum.localhost

bench --site erp.localhost add-to-hosts
bench --site masum.localhost add-to-hosts

bench get-app https://github.com/frappe/erpnext
bench get-app https://github.com/frappe/hrms

bench --site erp.localhost install-app erpnext hrms
bench --site masum.localhost install-app erpnext hrms

bench build