# k8s-wso2
Login to k8s cluster:
Do step by step: 
WSO2 on K8S 
-- namespace, service account 
cat ../pre-req/wso2ei-sa.yaml >> $k8s_obj_file
cat ../pre-req/wso2ei-secret.yaml >> $k8s_obj_file
--- configmap 
cat ../confs/wso2ei-conf.yaml >> $k8s_obj_file
cat ../confs/wso2ei-axis2-conf.yaml >> $k8s_obj_file
cat ../confs/wso2ei-ep-conf.yaml >> $k8s_obj_file
cat ../confs/wso2ei-ds-conf.yaml >> $k8s_obj_file
cat ../confs/wso2ei-analytics-worker-conf.yaml >> $k8s_obj_file
cat ../confs/wso2ei-analytics-dashboard-conf.yaml >> $k8s_obj_filevi

----mysql----------------- 
cat ../confs/wso2ei-mysql-db-conf.yaml >> $k8s_obj_file
cat ../mysql/wso2ei-mysql-deployment.yaml >> $k8s_obj_file
cat ../mysql/wso2ei-mysql-svc.yaml >> $k8s_obj_file

---- analytics worker ------------------
cat ../ei-analytics-worker/wso2ei-analytics-worker-deployment.yaml >> $k8s_obj_file
cat ../ei-analytics-worker/wso2ei-analytics-worker-svc.yaml >> $k8s_obj_file

---------analystic dashboard -------------------------------
cat ../ei-analytics-dashboard/wso2ei-analytics-dashboard-deployment.yaml >> $k8s_obj_file
cat ../ei-analytics-dashboard/wso2ei-analytics-dashboard-svc.yaml >> $k8s_obj_file

---------------------wso2 ei ----------------------------------------------
cat ../ei/wso2ei-deployment.yaml >> $k8s_obj_file
cat ../ei/wso2ei-svc.yaml >> $k8s_obj_file
cat ../ei/wso2ei-gateway-svc.yaml >> $k8s_obj_file



