# S3 Notes

## Important points
- Stores objects
- object size 0 bytes to 5 TB
- Offers unlimited storage
- S3 is universal name space
- Files stored in buckets
- Object class storage and does not support storage for operating systems and databases.
- HTTP 200 status code when upload complete successful 
- 
## Storage classes
- S3 - standard
- S3 - IA
- S3 - one zone - IA
- S3 - intelligent tering
- S3 - Glacier
- S3 - Glacier Deep archive
 
### Exam Tips
- Bucket name share a common name space
- No same bucket name as someone else (unique)
- Buckets are viewed globally, you can have buckets in individual region
- Content replication from one bucket to another using "cross region replication"
- Change of storage of class and encryption of object on the fly
- Restrict bucket access (control permission)
- Bucket policies (applied accross the whole bucket)
- Object policies (applied to individual files)
- IAM policies (Applied to users and groups)

## S3 Pricing

## What makes up the cost of S3
- Storage
- Request and data retension
- Data transfer
- Management & Replication

### Exam Question
1. Which tier of S3 should you use for given senario?
2. How to get best value out of S3

## S3 Security and encryption
- All buckets by default private
- You can set up access control to your buckets
-- Bucket policies (work at bucket level)
-- Access control list (it goes all the way to individual objects)
- Access logs can be stored in S3 buckets
- Encryption in transit = SSL/TLS
- Encryption at rest (where data is stored)
##### | S3 serverless | Client side |
| ---------------------------- | ----------- |
| (Managed by Amazon) | (Client side) |
|- S3 key managed keys - SSE-S3 |  |
|- AWS key management service |  | 
|- Managed keys -SSE - KMS | |
|- Severside encryption with customer provided keys - SSE-C | |

#### Type of encryption 
- Individual file encryption
- Bucket level encryption (much efficent compared to individual file encryption)

### S3 Versioning
- Stores all version objects
- Once enabled it cannot be disabled
- Intergrates life cycle rules
- Multifactor authorization to delete (additional layer of security)
- To make documents public each upload version needs permission
- 


