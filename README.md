# AWS Cloud Security Lab Series

Hands-on labs building a secure AWS environment step by step. Each lab adds one layer of protection, is tested to prove it works, and documents what it protects against.

**Author:** Ernestine Bineng, Security+ certified, focused on cloud and AI security

| Lab | Topic | What it shows |
|---|---|---|
| [Lab 0](lab-0-stop-using-root/) | Stop using root | Root protected with MFA, daily work from an MFA-protected admin user |
| [Lab 1](lab-1-least-privilege/) | Least privilege | A role that can only read one S3 bucket, MFA-required, validated and audited |
| [Lab 2](lab-2-guardrails/) | Guardrails | Bucket policy that blocks unencrypted connections, and a permissions boundary that holds even when too much access is attached |
| [Lab 3](lab-3-kms-data-protection/) | Data protection with KMS | A customer-managed key with rotation, default bucket encryption, and proof that reading data needs both S3 and key permissions |
| [Lab 4](lab-4-organizations-scp/) | Multi-account guardrails | AWS Organizations with a sandbox account and a service control policy that even the account's admins can't override |
| Lab 5 | Detection *(planned)* | CloudTrail and AWS Config rules for misconfigurations |
| Lab 6 | Automated response *(planned)* | GuardDuty → EventBridge → Lambda |
| Lab 7 | Infrastructure as code *(planned)* | Rebuilding the environment with CloudFormation or Terraform |

## How each lab is documented

1. **The problem**, in plain language
2. **What I built**, with the actual policies
3. **How I tested it**, with expected vs. actual results
4. **What it protects against**
5. **What I'd add next**

---

*All account IDs are replaced with AWS's placeholder `123456789012` or hidden in screenshots. No credentials are stored in this repository.*
