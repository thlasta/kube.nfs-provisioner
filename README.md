# kube.nfs-provisioner


echo "# kube.nfs-provisioner" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:thlasta/kube.nfs-provisioner.git
git push -u origin main

# Repo clonen
git clone git@github.com:thlasta/kube.nfs-provisioner.git

# Repo auschecken/holen
git pull git@github.com:thlasta/kube.nfs-provisioner.git

# Jump one folder up, and apply to the whole folder:
kubectl apply -f nfs-provisioner/

# Namespace "monitoring" anlegen
kubectl create namespace nfs-provisioner