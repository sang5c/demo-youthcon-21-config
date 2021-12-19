# demo-youthcon-21-config

ArgoCD에서는 이 repository를 감시합니다.

kustomize 빌드에 의해 `base/` 폴더의 yml 파일을 하나로 만들고, 특정 yml 속성을 덮어쓰기하여 ArgoCD에서 사용합니다.

### kustomize 빌드된 yml 확인하기
```shell
git clone https://github.com/sang5c/demo-youthcon-21-config
cd ./overlays/sample/
kubectl kustomize
```
kubectl 내장 kustomize를 사용하여 `overlays/sample/kustomization.yml` 파일에 정의된 image 속성으로 덮어쓰기 하는 것을 확인할 수 있습니다.
