# AWS Cloudtrail:
S3 Bucket Name: (anchor-$clientname-cloudtrail)  
Shared to any client accounts with s3:PutObject permissions
hostopia-dev-cloudtrail -yml

# Parameters:
1. Local
2. Development

# Format
WSTemplateFormatVersion: 2010-09-09

Description: Description of what the template is doing

Followed by an empty line

Followed by DEPLOYMENT, UPDATE and DELETE CLI commands for the template and local parameter file (see example

below). Any required capabilities will be added to the commands.

# Tags

CustomerId              1002966 (Catalyser)
Env                     prod, dev, sit, uat
Role                    webapp, db
