# ArgoCD
ArgoCD
Gitops-Git + operations, it is a modern approach to managing infra and application deployment using git
you stored your desired state in [ Kubernetes yaml files + Helm Chart + Terraform Code] stored in git, now automated system like ArgoCD, flux, continoulsy montoring the repo
and ensure your enviroment match the desired state.

#AgroCD#, it is a declarative ,gitops continous delivery tool for kubernetes, it provides automated deplyoment + Easy rollout + multicluster support+ visualization
Declarative means- manifest 

it is an automated tool when it always check that your current  state must be sync with a desired state.

#################current state= desired state ####################

There are two types of method we are using in gitops ,specially in ArgoCD
a) Pull Based Method b) Push based reconciliation 
Pull Based reconcilation Method- The system watches git and update itself 
Push Based - you tell the system to update

Pull based -- automatically tool argocd -continoulsy pull from the changes done in git repo and reconcile the system match the desired state
Push Based --- you pushed the changes in the git repo then trigger the desired changes in the infra and application


![Image Alt](https://github.com/ubuntomathur/ArgoCD/blob/main/argocd_architecture.webp)
