# Find Pod with vnetwork name
#### we have vnetwork with name `cali08a8f7340c7`
#### find cni with this command#### find cni with this command
```console
sudo ip a | grep -B 4 cali08a8f7340c7 
```

#### find Ip address of this vnetwork
```console
sudo ip netns exec cni-25a6977d-1d7d-cdc8-b931-0cf8d92b60da ip a
```
#### after find ip we try to find which pod has this IP
```console
 k get pods --all-namespaces -o wide --field-selector spec.nodeName=worker-02 | grep 10.233.113.171
```