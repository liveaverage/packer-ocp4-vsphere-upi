# Overview 



# Usage

  1. Set environment variable with password to access vCenter (or use Vault) for secure variables
     ````
     export VSPHERE_PASS="YourP@ssword"
     ````
  2. Update the variables in `rhcos.json` or pass as supplemental `-var` options as shown below
  3. Execute Packer to build the VM, which will shutdown when complete
     ```
     packer build -var "vcenter_password=${VSPHERE_PASS}" rhcos.json
     ``` 
  
