## Bind the edit role to the recruitment group

To create a Cluster Role Binding you must first log in to the [Kyma cluster](https://console.recruitment.kyma.pro/).  
Once you are logged in, follow the instructions below:

1. Go to _Global Permissions_ in the _Settings_ section.  
   It is on the left of the home screen of the cluster.
   
2. Click the **+ Create Binding** option.  
   It is in _Permissions_, in the _Cluster Role Bindings_ tab, on the top right.

3. Bind the **recruitment** group to the **edit** role in the pop-up window.  
   Enter `recruitment` in the _UserGroup_ field.  
   Select **edit** role from the _Role_ drop-down list. Start typing for the role to appear faster.
   
4. Click on **Save**.  
   
Your newly created binding now appears in the list of bindings in _Cluster Role Bindings_. 



## Namespaces

A Namespace is one of multiple virtual clusters backed by the same physical cluster.
It provides a scope for names of resources, which must be unique within a Namespace, but not across Namespaces. 
This allows for increasing the security and organization of your cluster by dividing it into smaller units. 
These units can then be used for different purposes, such as development and testing.  
Namespaces are intended for environments with many users from multiple teams, or projects, and Kubernetes and Kyma rely heavily on them.

Kyma comes with three Namespaces available for users, as well as four default Kyma Namespaces for system-related purposes.  
The default Namespaces are: `kyma-system`, `kyma-integration`, `kyma-installer`, and `istio-system`, and the user cannot modify or remove them.  
The pre-configured Namespaces for users are: `production`, `qa`, and `stage`, and they are ready to use.  

