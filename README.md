# CICD-Test
##install-prereuisities.yml  is a cloud formation template which deploys 3 Windows VMs. 
> There is an userdata which runs inside each VM. For which it pulls in the powershell script which is store in AWS s3( which is made public)
> The same powershell can be directly written in the userdata but to reduce the line of code i have added it on s3 bucket
  * https://s3.amazonaws.com/testing-java-jdk/countries.ps1
  * https://s3.amazonaws.com/testing-java-jdk/airports101.ps1
  * https://s3.amazonaws.com/testing-java-jdk/airports110.ps1
  * https://s3.amazonaws.com/testing-java-jdk/jdk-8u181-windows-x64.exe (jdk exe)
> Currently in the template it download the respective pwershell file and runs in their resective VMs
## Parameters.json file is mainly for automation via VSTS.