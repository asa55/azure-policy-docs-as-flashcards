##

Azure Policy helps to enforce organizational standards and to assess `_____` at-scale.

%

Azure Policy helps to enforce organizational standards and to assess **compliance** at-scale.

##

Through its compliance `_____`, Azure Policy provides an aggregated view to evaluate the overall state of the environment, with the ability to drill down to the per-resource, per-policy granularity. It also helps to bring your resources to compliance through bulk remediation for existing resources and automatic remediation for new resources.

%

Through its compliance **dashboard**, Azure Policy provides an aggregated view to evaluate the overall state of the environment, with the ability to drill down to the per-resource, per-policy granularity. It also helps to bring your resources to compliance through bulk remediation for existing resources and automatic remediation for new resources.

##

Policy definitions for these common use cases are already available in your Azure environment as built-ins to help you get started.

Common use cases for Azure Policy include implementing governance for

- `_____`
- `_____`
- `_____`
- `_____`
- `_____`

%

- resource consistency
- regulatory compliance
- security
- cost
- and management

##

Some useful governance actions you can enforce with Azure Policy include:

- Ensuring your team deploys Azure resources only to allowed `_____`
- Enforcing the consistent application of taxonomic `_____`
- Requiring resources to send diagnostic logs to a `_____` workspace

%

- Ensuring your team deploys Azure resources only to allowed **regions**
- Enforcing the consistent application of taxonomic **tags**
- Requiring resources to send diagnostic logs to a **Log Analytics** workspace

##

With the introduction of Azure `_____`, you can extend your policy-based governance across different cloud providers and even to your local datacenters.

%

With the introduction of Azure **Arc**, you can extend your policy-based governance across different cloud providers and even to your local datacenters.

##

All Azure Policy data and objects are encrypted at

%

rest

##

Azure Policy evaluates resources and actions in Azure by comparing the properties of those resources to business rules. These business rules, described in JSON format, are known as policy

%

definitions

##

To simplify management, several business rules (policy definitions) can be grouped together to form a policy initiative (sometimes called a policySet). Once your business rules have been formed, the policy definition or initiative is assigned to any scope of resources that Azure supports, such as 

- `_____`
- `_____`
- `_____`
- `_____`

%

- management groups
- subscriptions
- resource groups
- or individual resources

##

The assignment of a policy definition or initiative to a scope of resources that Azure supports applies to all resources within the Resource Manager scope of that assignment. If necessary, subscopes can be

%

excluded

##

Azure Policy uses a `_____` format to form the logic the evaluation uses to determine whether a resource is compliant or not. 

%

Azure Policy uses a **JSON** format to form the logic the evaluation uses to determine whether a resource is compliant or not. 

##

Policy definitions include metadata and the policy `_____`. The defined `_____` can use functions, parameters, logical operators, conditions, and property aliases to match exactly the scenario you want. The policy `_____` determines which resources in the scope of the assignment get evaluated.

%

Policy definitions include metadata and the policy **rule**. The defined **rule** can use functions, parameters, logical operators, conditions, and property aliases to match exactly the scenario you want. The policy **rule** determines which resources in the scope of the assignment get evaluated.

##

Resources are evaluated at specific times during the resource lifecycle, the policy assignment lifecycle, and for regular ongoing compliance evaluation. The following are the times or events that cause a resource to be evaluated:

- A `_____` is created or updated in a scope with a policy assignment.
- A policy or initiative is newly `_____` to a scope.
- A policy or initiative already assigned to a scope is `_____`.
- During the standard compliance evaluation cycle, which occurs once every `_____` hours.

%

- A **resource** is created or updated in a scope with a policy assignment.
- A policy or initiative is newly **assigned** to a scope.
- A policy or initiative already assigned to a scope is **updated**.
- During the standard compliance evaluation cycle, which occurs once every **24** hours.

##

Business rules for handling non-compliant resources vary widely between organizations. Examples of how an organization wants the platform to respond to a non-compliant resource include:

- Deny the `_____` change
- Log the change to the `_____`
- Alter the `_____` before the change
- Alter the `_____` after the change
- Deploy related compliant `_____`
- Block actions on `_____`

%

- Deny the **resource** change
- Log the change to the **resource**
- Alter the **resource** before the change
- Alter the **resource** after the change
- Deploy related compliant **resources**
- Block actions on **resources**

##

Azure Policy makes business responses possible through the application of `_____`. `_____` are set in the policy rule portion of the policy definition.

While these `_____` primarily affect a resource when the resource is created or updated, Azure Policy also supports dealing with existing non-compliant resources without needing to alter that resource.

%

Azure Policy makes business responses possible through the application of **effects**. **Effects** are set in the policy rule portion of the policy definition.

While these **effects** primarily affect a resource when the resource is created or updated, Azure Policy also supports dealing with existing non-compliant resources without needing to alter that resource.

##

There are a few key differences between Azure Policy and Azure

%

role-based access control (Azure RBAC)

##

Azure Policy evaluates state by examining properties on `_____` that are represented in `_____` Manager and properties of some `_____` Providers. Azure Policy ensures that `_____` state is compliant to your business rules without concern for who made the change or who has permission to make a change. Azure Policy through DenyAction effect can also block certain actions on `_____`. Some Azure Policy `_____`, such as policy definitions, initiative definitions, and assignments, are visible to all users. This design enables transparency to all users and services for what policy rules are set in their environment.

%

Azure Policy evaluates state by examining properties on **resources** that are represented in **Resource** Manager and properties of some **Resource** Providers. Azure Policy ensures that **resource** state is compliant to your business rules without concern for who made the change or who has permission to make a change. Azure Policy through DenyAction effect can also block certain actions on **resources**. Some Azure Policy **resources**, such as policy definitions, initiative definitions, and assignments, are visible to all users. This design enables transparency to all users and services for what policy rules are set in their environment.

##

Azure `_____` focuses on managing user actions at different scopes. If control of an action is required based on user information, then Azure `_____` is the correct tool to use. Even if an individual has access to perform an action, if the result is a non-compliant resource, Azure Policy still blocks the create or update.

%

Azure **RBAC** focuses on managing user actions at different scopes. If control of an action is required based on user information, then Azure **RBAC** is the correct tool to use. Even if an individual has access to perform an action, if the result is a non-compliant resource, Azure Policy still blocks the create or update.

##

The combination of Azure RBAC and Azure Policy provides full scope control in

%

Azure

##

Azure Policy has several permissions, known as operations, in two Resource Providers:

- Microsoft.`_____`
- Microsoft.`_____`

%

- Microsoft.**Authorization**
- Microsoft.**PolicyInsights**

##

For Azure RBAC permissions in Azure Policy, many built-in `_____` grant permission to Azure Policy resources. The `Resource Policy Contributor` `_____` includes most Azure Policy operations. `Owner` has full rights. Both `Contributor` and `Reader` have access to all read Azure Policy operations.

%

For Azure RBAC permissions in Azure Policy, many built-in **roles** grant permission to Azure Policy resources. The `Resource Policy Contributor` **role** includes most Azure Policy operations. `Owner` has full rights. Both `Contributor` and `Reader` have access to all read Azure Policy operations.

##

For Azure RBAC permissions in Azure Policy, `Contributor` may trigger resource remediation, but can't create or update definitions and assignments. `User Access Administrator` is necessary to grant the `_____` on `deployIfNotExists` or `modify` assignments necessary permissions.

%

For Azure RBAC permissions in Azure Policy, `Contributor` may trigger resource remediation, but can't create or update definitions and assignments. `User Access Administrator` is necessary to grant the **managed identity** on `deployIfNotExists` or `modify` assignments necessary permissions.

##

All Policy objects, including definitions, initiatives, and assignments, will be `_____` to all roles over its scope. For example, a Policy assignment scoped to an Azure subscription will be `_____` by all role holders at the subscription scope and below.

%

All Policy objects, including definitions, initiatives, and assignments, will be **readable** to all roles over its scope. For example, a Policy assignment scoped to an Azure subscription will be **readable** by all role holders at the subscription scope and below.

##

If none of the built-in roles have the permissions required, create a

%

custom role

##

Azure Policy operations can have a significant `_____` on your Azure environment. Only the minimum set of permissions necessary to perform a task should be assigned and these permissions should not be granted to users who do not need them.

%

Azure Policy operations can have a significant **impact** on your Azure environment. Only the minimum set of permissions necessary to perform a task should be assigned and these permissions should not be granted to users who do not need them.

##

The managed identity of a `deployIfNotExists` or `modify` policy assignment needs enough `_____` to create or update targeted resources.

%

The managed identity of a `deployIfNotExists` or `modify` policy assignment needs enough **permissions** to create or update targeted resources.

##

Azure Virtual Network Manager (preview) enables you to apply consistent management and security `_____` to multiple Azure virtual networks (VNets) throughout your cloud infrastructure. Azure Virtual Network Manager (AVNM) dynamic groups use Azure `_____` definitions to evaluate VNet membership in those groups.

%

Azure Virtual Network Manager (preview) enables you to apply consistent management and security **policies** to multiple Azure virtual networks (VNets) throughout your cloud infrastructure. Azure Virtual Network Manager (AVNM) dynamic groups use Azure **Policy** definitions to evaluate VNet membership in those groups.

##

To create, edit, or delete Azure Virtual Network Manager dynamic group policies, you need:

- Read and write Azure RBAC permissions to the underlying policy
- Azure RBAC permissions to join the network group (Note: Classic Admin authorization is not supported)

Specifically, the required resource provider permission is

`Microsoft.Network/networkManagers/networkGroups/_____/_____`

%

`Microsoft.Network/networkManagers/networkGroups/join/action`

##

To modify Azure Virtual Network Manager (AVNM) dynamic groups, you must be granted access via Azure RBAC role assignment only. Classic Admin/legacy authorization is not supported; this means if your account were assigned only the co-administrator subscription role, you'd have no permissions on

%

AVNM dynamic groups

##

Azure Policy evaluates all Azure resources at or below `_____`-level, including Arc enabled resources. For certain resource providers such as Machine configuration, Azure Kubernetes Service, and Azure Key Vault, there's a deeper integration for managing settings and objects.

%

Azure Policy evaluates all Azure resources at or below **subscription**-level, including Arc enabled resources. For certain resource providers such as Machine configuration, Azure Kubernetes Service, and Azure Key Vault, there's a deeper integration for managing settings and objects.

##

Recommendation for managing policies:

Start with an `_____` or `_____` effect instead of an enforcement (`deny`, `modify`, `deployIfNotExist`) effect to track impact of your policy definition on the resources in your environment. If you have scripts already in place to autoscale your applications, setting an enforcement effect may hinder such automation tasks already in place.

%

Start with an `audit` or `auditIfNotExist` effect instead of an enforcement (`deny`, `modify`, `deployIfNotExist`) effect to track impact of your policy definition on the resources in your environment. If you have scripts already in place to autoscale your applications, setting an enforcement effect may hinder such automation tasks already in place.

##

Recommendation for managing policies:

Consider organizational `_____` when creating definitions and assignments. We recommend creating definitions at higher levels such as the management group or subscription level. Then, create the assignment at the next child level. If you create a definition at a management group, the assignment can be scoped down to a subscription or resource group within that management group.

%

Consider organizational **hierarchies** when creating definitions and assignments. We recommend creating definitions at higher levels such as the management group or subscription level. Then, create the assignment at the next child level. If you create a definition at a management group, the assignment can be scoped down to a subscription or resource group within that management group.

##

Recommendation for managing policies:

We recommend creating and assigning `_____` definitions even for a single policy definition. For example, you have policy definition _policyDefA_ and create it under `_____` definition _initiativeDefC_. If you create another policy definition later for _policyDefB_ with goals similar to _policyDefA_, you can add it under _initiativeDefC_ and track them together.
  - Once you've created an `_____` assignment, policy definitions added to the `_____` also become part of that `_____`'s assignments.
  - When an `_____` assignment is evaluated, all policies within the `_____` are also evaluated. If you need to evaluate a policy individually, it's better to not include it in an `_____`.

%

We recommend creating and assigning **initiative** definitions even for a single policy definition. For example, you have policy definition _policyDefA_ and create it under **initiative** definition _initiativeDefC_. If you create another policy definition later for _policyDefB_ with goals similar to _policyDefA_, you can add it under _initiativeDefC_ and track them together.
  - Once you've created an **initiative** assignment, policy definitions added to the **initiative** also become part of that **initiative**'s assignments.
  - When an **initiative** assignment is evaluated, all policies within the **initiative** are also evaluated. If you need to evaluate a policy individually, it's better to not include it in an **initiative**.

##

Recommendation for managing policies:

Manage Azure Policy resources as `_____` with manual reviews on changes to policy definitions, initiatives, and assignments.

%

Manage Azure Policy resources as **code** with manual reviews on changes to policy definitions, initiatives, and assignments.

##

The journey of creating and implementing a policy in Azure Policy begins with creating a policy `_____`. Every policy `_____` has conditions under which it's enforced. And, it has a defined effect that takes place if the conditions are met.

%

The journey of creating and implementing a policy in Azure Policy begins with creating a policy **definition**. Every policy **definition** has conditions under which it's enforced. And, it has a defined effect that takes place if the conditions are met.

##

In Azure Policy, we offer several built-in policies that are available by default. For example:

- Allowed Storage Account SKUs (`_____`): Determines if a storage account being deployed is within a set of SKU sizes. Its effect is to `_____` all storage accounts that don't adhere to the set of defined SKU sizes.
- Allowed Resource Type (`_____`): Defines the resource types that you can deploy. Its effect is to `_____` all resources that aren't part of this defined list.
- Allowed Locations (`_____`): Restricts the available locations for new resources. Its effect is used to enforce your geo-compliance requirements.
- Allowed Virtual Machine SKUs (`_____`): Specifies a set of virtual machine SKUs that you can deploy.
- Add a tag to resources (`_____`): Applies a required tag and its default value if it's not specified by the deploy request.
- Not allowed resource types (`_____`): Prevents a list of resource types from being deployed.

%

- Allowed Storage Account SKUs (**Deny**): Determines if a storage account being deployed is within a set of SKU sizes. Its effect is to **deny** all storage accounts that don't adhere to the set of defined SKU sizes.
- Allowed Resource Type (**Deny**): Defines the resource types that you can deploy. Its effect is to **deny** all resources that aren't part of this defined list.
- Allowed Locations (**Deny**): Restricts the available locations for new resources. Its effect is used to enforce your geo-compliance requirements.
- Allowed Virtual Machine SKUs (**Deny**): Specifies a set of virtual machine SKUs that you can deploy.
- Add a tag to resources (**Modify**): Applies a required tag and its default value if it's not specified by the deploy request.
- Not allowed resource types (**Deny**): Prevents a list of resource types from being deployed.

##

To implement policy definitions (both built-in and custom definitions), you'll need to `_____` them. You can `_____` any of these policies through the Azure portal, PowerShell, or Azure CLI.

%

To implement policy definitions (both built-in and custom definitions), you'll need to **assign** them. You can **assign** any of these policies through the Azure portal, PowerShell, or Azure CLI.

##

Policy `_____` happens with several different actions, such as policy assignment or policy updates.

%

Policy **evaluation** happens with several different actions, such as policy assignment or policy updates.

##

Policy `_____` help simplify your policy management by reducing the number of policy definitions you must create. You can define `_____` when creating a policy definition to make it more generic. Then you can reuse that policy definition for different scenarios. You do so by passing in different values when assigning the policy definition. For example, specifying one set of locations for a subscription.

`_____` are defined when creating a policy definition. When a `_____` is defined, it's given a name and optionally given a value. For example, you could define a `_____` for a policy titled location. Then you can give it different values such as EastUS or WestUS when assigning a policy.

%

Policy **parameters** help simplify your policy management by reducing the number of policy definitions you must create. You can define **parameters** when creating a policy definition to make it more generic. Then you can reuse that policy definition for different scenarios. You do so by passing in different values when assigning the policy definition. For example, specifying one set of locations for a subscription.

**Parameters** are defined when creating a policy definition. When a **parameter** is defined, it's given a name and optionally given a value. For example, you could define a **parameter** for a policy titled location. Then you can give it different values such as EastUS or WestUS when assigning a policy.

##

An `_____` definition is a collection of policy definitions that are tailored toward achieving a singular overarching goal. `_____` definitions simplify managing and assigning policy definitions. They simplify by grouping a set of policies as one single item. For example, you could create an `_____` titled Enable Monitoring in Microsoft Defender for Cloud, with a goal to monitor all the available security recommendations in your Microsoft Defender for Cloud instance.

%

An **initiative** definition is a collection of policy definitions that are tailored toward achieving a singular overarching goal. **Initiative** definitions simplify managing and assigning policy definitions. They simplify by grouping a set of policies as one single item. For example, you could create an **initiative** titled Enable Monitoring in Microsoft Defender for Cloud, with a goal to monitor all the available security recommendations in your Microsoft Defender for Cloud instance.

##

The SDK, such as Azure CLI and Azure PowerShell, use properties and parameters named `_____` to refer to initiatives.

%

The SDK, such as Azure CLI and Azure PowerShell, use properties and parameters named `PolicySet` to refer to initiatives.

##

Like policy parameters, initiative parameters help simplify initiative management by reducing redundancy. Initiative parameters are parameters being used by the policy definitions within the

%

initiative

##

When creating value options in an initiative definition, you're unable to input a different value during the initiative assignment because it's not part of the

%

list

##

An `_____` is a policy definition or initiative that has been assigned to a specific scope. This scope could range from a management group to an individual resource. The term scope refers to all the resources, resource groups, subscriptions, or management groups that the definition is assigned to. `_____` are inherited by all child resources. This design means that a definition applied to a resource group is also applied to resources in that resource group. However, you can exclude a subscope from the `_____`.

%

An **assignment** is a policy definition or initiative that has been assigned to a specific scope. This scope could range from a management group to an individual resource. The term scope refers to all the resources, resource groups, subscriptions, or management groups that the definition is assigned to. **Assignments** are inherited by all child resources. This design means that a definition applied to a resource group is also applied to resources in that resource group. However, you can exclude a subscope from the **assignment**.

##

Example: at the subscription scope, you can assign a `_____` that prevents the creation of networking resources. You could exclude a resource group in that subscription that is intended for networking infrastructure. You then grant access to this networking resource group to users that you trust with creating networking resources.

%

Example: at the subscription scope, you can assign a **definition** that prevents the creation of networking resources. You could exclude a resource group in that subscription that is intended for networking infrastructure. You then grant access to this networking resource group to users that you trust with creating networking resources.

##

Example: You might want to assign a resource type allowlist definition at the `_____` level. Then you assign a more permissive policy (allowing more resource types) on a child `_____` or even directly on subscriptions. However, this example wouldn't work because Azure Policy is an explicit deny system. Instead, you need to exclude the child `_____` or subscription from the `_____`-level assignment. Then, assign the more permissive definition on the child `_____` or subscription level. If any assignment results in a resource getting denied, then the only way to allow the resource is to modify the denying assignment.

%

Example: You might want to assign a resource type allowlist definition at the **management group** level. Then you assign a more permissive policy (allowing more resource types) on a child **management group** or even directly on subscriptions. However, this example wouldn't work because Azure Policy is an explicit deny system. Instead, you need to exclude the child **management group** or subscription from the **management group**-level assignment. Then, assign the more permissive definition on the child **management group** or subscription level. If any assignment results in a resource getting denied, then the only way to allow the resource is to modify the denying assignment.

##

Policy assignments always use the `_____` state of their assigned definition or initiative when evaluating resources. If a policy definition that is already assigned is changed all existing assignments of that definition will use the updated logic when evaluating.

%

Policy assignments always use the **latest** state of their assigned definition or initiative when evaluating resources. If a policy definition that is already assigned is changed all existing assignments of that definition will use the updated logic when evaluating.

##

The maximum count of Policy Definitions for a management group, subscription, resource group, or individual resource is

%

500

##

The maximum count of Initiative Definitions for a management group, subscription, resource group, or individual resource is

%

200

##

The maximum count of Initiative Definitions for a Tenant is

%

2,500

##

The maximum count of Policy or Initiative Assignments for a management group, subscription, resource group, or individual resource is

%

200

##

The maximum count of Exemptions for a management group, subscription, resource group, or individual resource is

%

1,000

##

The maximum count of Parameters for a Policy Definition is

%

20

##

The maximum count of Policies for an Initiative Definition is

%

1,000

##

The maximum count of Parameters for an Initiative Definition is

%

300

##

The maximum count of Exclusions for Policy or Initiative Assignments is

%

400

##

The maximum count of Nested Conditionals for a Policy Rule is

%

512

##

The maximum count of Resources for a Remediation Task is

%

50,000

##

The maximum count of Bytes for a Policy Definition, Initiative, or Assignment request body is

%

1,048,576 Bytes, approx. 1MB
