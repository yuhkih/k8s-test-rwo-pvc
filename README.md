# k8s-test-rwo-pvc

yamls to test PV (PVC :Read Write Once) access from multiiple pod 

Memos:
1) be aware of setting nodeSelector value to the environment at the time of experiment
2) "storageClassName: thin" in PVC definition is VMware VMDK in-tree driver's default value for OpenShift 4.9 (maybe in-tree storage driver be removed in later version of OpenShift)

*Label nodes for the test ilke the followings*
kubectl label nodes ocp48-h49p6-worker-2dmjq worker=worker1
kubectl label nodes ocp48-h49p6-worker-9n5fg worker=worker2
kubectl label nodes ocp48-h49p6-worker-l7lnn worker=worker3

