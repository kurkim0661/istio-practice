# Istio test

minikube service 를 통해서 특정 service를 local로 port-forwarding을 해야 접속이 가능... 
nodeport로 돼있어서 minikube ip와 port 조합으로 접근을 할 수 있을 것으로 생각 했지만 접속이 되지 않는 문제가 있었다.
확인해보니 minikube --vm-driver=none로 설정해줘야 한다고함 default로 virtualbox가 잡히게 되는데 이러먼 main host에서 접근하기 위한 추가 configuration 작업을 해줘야 한다고함.