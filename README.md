# _Terraform Module: terraform-module-aws-rds-cluster-parameter-group_


## _General_

_This module can be used to deploy a_ _**Database Parameter Group** on **AWS** Cloud Provider......_


---

## _Prerequisites_

_This module needs **Terraform 0.12.20** or newer._
_You can download the latest Terraform version from_ [_here_](https://www.terraform.io/downloads.html).



---

## _Features Branches_

_Below we are able to check the resources that are being created as part of this module call:_

- _**Database Parameter Group**_


---

## _Usage_

## _Using this repo_

_To use this module, add the following call to your code:_

```tf
module "rds_cluster_parameter_group" {
  source = "git::https://github.com/nitinda/terraform-module-aws-rds-cluster-parameter-group.git?ref=master"


}
```


---

## _Inputs_

_The variables required in order for the module to be successfully called from the deployment repository are the following:_

|**_Variable_** | **_Description_** | **_Type_** | **_Argument Status_** |
|:----|:----|-----:|:---:|
| **_name\_prefix_** | _Creates a unique name_ | _string_ |
| **_description_** | _The description of the DB subnet group_ | _string_ | **_Required_** |
| **_family_** | _The family of the DB cluster_ | _string_ | **_Required_** |
| **_parameter_** | _A list of DB parameters to apply_ | _any_ | **_Optional (Default [])_** |
| **_tags_** | _Resource tags_ | _map(string)_ | **_Required_** |


---


## _Outputs_

### _General_

_This module has the following outputs:_


* **_id_**
* **_arn_**


### _Usage_

_In order for the variables to be accessed at module level please use the syntax below:_

```tf
module.<module_name>.<output_variable_name>
```


_The output variable is able to be accessed through terraform state file using the syntax below:_

```tf
data.terraform_remote_state.<layer_name>.<output_variable_name>
```

---



## _Authors_

_Module maintained by Module maintained by the -_ **_Nitin Das_**