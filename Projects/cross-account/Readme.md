---------------------------------------------------------------------------------------------------------------------
1. Roles 

. Cross-Account Role (All Accounts)
. Cloudformation Role (All Accounts)

2. CICD 

.  Cloudformation ---> Artifact(V)--->S3 BUcket Policy(ME)/CodeComit(v)/CodeBuild(v)-->cfn-lint/Pipeline(Me)/Pipeline(me) Role

3. Pipeline--Structure

. 1. Source --> codecommit/kms/role

. 2. Build --> cfn-lint
-----------------------------------------------------------------------------------------------------------------------
. 3. Roles Stage

    a. Roles(4) sec,dev,sta,prod 

. 4. Security Stage 

    a. Infra b. app c. LambdaVpcSg 

. 5. Dev

    a. Infra b. app c. db d. waf 

. 6. Staging

    a. Infra b. app c. db d. waf 

. 7. Production

    a. Infra b. app c. db d. waf 

. 8. Security-2

    a. LambdaPeeringID b. PeerRouting 

. 9. Backup

    a. Cloudtrail  b. Config c. Cloudhealth d. Datadog e. SNS 
-----------------------------------------------------------------------------------------------------------------------
. S3 Bucket 