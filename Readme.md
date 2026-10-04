EC2:
- Instance type: t3.micro
- OS: Amazon Linux 2023
- Region: us-east-1
- Instance name: SessionManager-Demo

Systems Manager:
- Session Manager configuration
- SSM Agent commands
- CloudWatch log group name
- S3 bucket configuration/documentation

IAM:
- Policy JSON/documentation, if sanitized
- Role/Sessionmanager name such as LabRole

S3:
- Bucket purpose: Session Manager session logs
- Bucket name: bharath-session-manager-logs-2026
- Region: us-east-1
- Encryption: Enabled
- Public access: Blocked
- Session Manager S3 logging: Enabled