# commvault-aws-role-deployment
Commvault required roles for AWS (Single account or Organization)

Deploy required roles for Commvault backup in administrative/service account and member accounts (For AWS Organization). Deploy #1 as cloudformation stack in the account you plan to use as the service account. #2 can be deployed individually in each (any account that has resources to be backedup) member account or as stack-set 

#1. vsa_assume_admin_role.yaml - Commvault role to be associated with management node (Ref: Commvault example demoEC2role.json)
#2. omni_vsa_tenant_role.yaml - Role and permissions required by Commvault in Tenant account
