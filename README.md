# wkspopular2


oc new-project cp4i

oc create secret docker-registry ibm-entitlement-key --docker-username=cp --docker-password=eyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJJQk0gTWFya2V0cGxhY2UiLCJpYXQiOjE1Nzg2ODgyNTksImp0aSI6IjdmYmZiMTM3NGFlNTQyOWZhOTM2MDdlOGUwYTcyNDU5In0.sd_sOTRpEsR3u9cxV_rR4jsxq4tuN6YHcyVmE8AngcQ --docker-server=cp.icr.io -n cp4i



oc get secrets -n ibm-common-services platform-auth-idp-credentials -ojsonpath='{.data.admin_password}' | base64 --decode && echo "" --------> GET CLOUD PAK DASHBOARD
