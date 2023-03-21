# magma-deployer

Quick Install:
```bash
sudo bash -c "$(curl -sL https://github.com/magma/magma-deployer/raw/master/deploy-orc8r.sh)"
```

Switch to `magma` user after deployment has finsished:
```bash
sudo su - magma
```

Once all pods are ready, setup NMS login:
```bash
cd ~/magma-galaxy
ansible-playbook config-orc8r.yml
```

You can get your `rootCA.pem` file from the following location:
```bash
cat ~/magma-galaxy/secrets/rootCA.pem
```
