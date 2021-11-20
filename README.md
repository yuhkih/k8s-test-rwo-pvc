# k8s-test-rwo-pvc

yamls to test PV (PVC :Read Write Once) access from multiiple pod 

Memos:
1) be aware of setting nodeSelector value to the environment at the time of experiment
2) "storageClassName: thin" in PVC definition is VMware VMDK in-tree driver default value for OpenShift 4.9 (maybe in-tree driver be removed in later version)
