# kube_space project

①仮想マシン起動
minikube start

②デプロイメントの定義ファイル読み込み
kubectl apply -f deployment/httpd/apa000dep.yml

③Podが作られていることの確認
kubectl get pods

④サービスの定義ファイルの読み込み
kubectl apply -f service/httpd/apa000ser.yml

⑤サービスが作られていることの確認
kubectl get services

⑥デプロイメントの削除
kubectl delete -f deployment/httpd/apa000dep.yml

⑦サービスの削除
kubectl delete -f service/httpd/apa000ser.yml